# jsDelta2017
GPU implementation of delta mush for Maya 2017

A few changes in the GPU override class, so I'm keeping 2017 in a different repo for now.

The file jsDelta.cl MUST be in the same folder alongside the compiled plugin for GPU override to work.

Loading plugin adds command "jsDeltaCmd()" to maya.cmds. Select target mesh and run command from the script editor. You can also create a bare node with deformer(type="jsDelta").

Version for 2016.5 coming soon.

2017 Changes:
- getOpenCLCommandQueue has been replaced with getMayaDefaultOpenCLCommandQueue
- MGPUDeformerRegistrationInfo class now requires two separate validation functions instead of validateNode()
- the 2017 validate functions (mentioned I think in the 2016 docs but I never implemented them) are validateNodeValues() and validateNodeInGraph()
