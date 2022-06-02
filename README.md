# Roadmap/subprojects of the new S4TF

> [tensorflow/swift](https://github.com/tensorflow/swift) is archived, but the project lives on.

The resurrection of Swift for TensorFlow touches on several disparate topics. This project ranges from bypassing the iOS sandbox - to making OpenCL bindings - to building IDE plugins. Here is an growing list of code bases created for the purpose of bringing back S4TF. I am developing and maintaining all of this simultaneously, and can barely handle it alone. Any help is greatly appreciated!

- [s4tf/s4tf](https://github.com/s4tf/s4tf) - The current head branch of S4TF, forked from tensorflow/swift-apis. I plan to merge the awesome-looking [former README](https://github.com/s4tf/s4tf-docs) of tensorflow/swift into this repo.
- [philipturner/swift-colab](https://github.com/philipturner/swift-colab) - The first large-scale task revolving around S4TF and a very useful tool in its own right. Brought Swift back to Google Colaboratory after the <s>official</s> predecessor Jupyter kernel was "sunset".
- [philipturner/swift-opencl](https://github.com/philipturner/swift-opencl) - Laying groundwork for the future OpenCL backend. This will let me create custom OpenCL kernels, complementing the fast matrix multiplication kernels provided by [artyom-beilis/dlprimitives](https://github.com/artyom-beilis/dlprimitives).
- [swift4science/s4tf-docker](https://gitlab.com/swift4science/s4tf-docker) - Thanks to this repo, we know how to compile S4TF again. It has evolved into the [S4TF build script](https://gist.github.com/philipturner/7aa063af04277d463c14168275878511), currently hosted as a GitHub gist. I will eventually embed this gist into S4TF documentation.
- [philipturner/differentiation](https://github.com/philipturner/differentiation) - Bypassing the fact that AutoDiff is disabled on release toolchains. This allows it to [run on iOS](https://github.com/philipturner/differentiation-ios-demo) - good news for anyone whose iPhone or iPad has a more powerful GPU than their old Intel Mac.
- [philipturner/swift-reflection-mirror](https://github.com/philipturner/swift-reflection-mirror) - Reimplemented a runtime reflection feature that was strangely gated behind an inaccessible API. This briefly gave me a [good hearty scare](https://forums.swift.org/t/the-future-of-reflective-programming-in-swift/54956/17). Apple, why?
- The Metal backend is prototyped in private repositories, but they may become public in the future. 

The [s4tf](https://github.com/philipturner/s4tf) organization hosts inactive repositories formerly hosted by the [tensorflow](https://github.com/tensorflow) organization. Anyone is free to become a member, even just as something symbolic. Just contact me over GitHub or email to request to join.

## Not directly related

- [philipturner/metal-fft](https://github.com/philipturner/metal-fft) has turned into satire of Google's archiving of S4TF.
- We finally have a community-based [working group](https://forums.swift.org/t/formalizing-a-numerical-ml-working-group/45553) for using Swift for numerical computing and machine learning.
- [vojtamolda/tensor-thumbnail](https://github.com/vojtamolda/tensor-thumbnail) has removed its archive tombstone, and I seek to integrate it into mainline S4TF.
