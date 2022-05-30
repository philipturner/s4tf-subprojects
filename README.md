# Roadmap/subprojects of the new S4TF

The recent activity around Swift for TensorFlow touches on several disparate topics. Subprojects involve everything from bypassing Apple's iOS sandbox to making OpenCL kernels for machine learning. Here is an growing list of code created for the purpose of resurrecting S4TF:

- [s4tf/s4tf](https://github.com/s4tf/s4tf) - The new head branch of S4TF, forked from [tensorflow/swift-apis](https://github.com/tensorflow/swift-apis). I will eventually merge the awesome-looking README of [s4tf-docs](https://github.com/s4tf/s4tf-docs) into this repo.
- [swift4science/s4tf-docker](https://gitlab.com/swift4science/s4tf-docker) - Thanks to this repo, we know how to compile S4TF again. It is incorporated into the [S4TF build script](https://gist.github.com/philipturner/7aa063af04277d463c14168275878511), currently hosted as a GitHub gist. The gist will eventually be embedded into S4TF documentation.
- philipturner/differentiation
- philipturner/swift-colab
- philipturner/swift-reflection-mirror
- [philipturner/swift-opencl](https://github.com/philipturner/swift-opencl) - Laying groundwork for the future OpenCL backend for S4TF. This will let me create custom OpenCL kernels, complementing the fast matrix multiplication kernels provided by [artyom-beilis/dlprimitives](https://github.com/artyom-beilis/dlprimitives).
- The Metal backend is prototyped in private repositories, but they may become public in the future.

The [s4tf](https://github.com/philipturner/s4tf) organization hosts inactive repositories formerly hosted by the [tensorflow](https://github.com/tensorflow) organization. Anyone is free to become a member, even as a symbolic gesture. Just contact me over GitHub or email.
