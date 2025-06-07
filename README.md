# csi-vae with PyTorch

This repository contains a modified version of the original csi-vae project, which was initially developed in TensorFlow. The main changes introduced include:

**Migration to PyTorch :**
The code has been completely rewritten in PyTorch, preserving the original model's architecture and logic while taking advantage of PyTorch's flexibility and modularity.

**Increased Flexibility :**
Dynamic antenna selection: It is now possible to select one, multiple specific, or all available antennas as input to the model through a simple configuration setting.

Configurable activation functions: Users can easily choose the type of activation function (ReLU, LeakyReLU, ELU, etc.) to use in the model by leveraging the torch.nn modules.

**Configuration via JSON5 :**
Model and training parameters are now managed through a config.json5 file, which allows comments and greater flexibility when defining parameters. This makes tuning and using the code much simpler and more readable.

**Secure Saving with SafeTensor :**
Trained models are saved using SafeTensor, a secure and efficient format for tensor serialization.
