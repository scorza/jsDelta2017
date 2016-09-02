# jsDelta2017
GPU implementation of delta mush for Maya 2017

A few changes in the GPU override class, so I'm keeping 2017 in a different repo for now.

- getOpenCLCommandQueue has been replaced with getMayaDefaultOpenCLCommandQueue
- MGPUDeformerRegistrationInfo class now requires two separate validation functions instead of validateNode()
- the 2017 validate functions (mentioned I think in the 2016 docs but I never implemented them) are validateNodeValues() and validateNodeInGraph()
