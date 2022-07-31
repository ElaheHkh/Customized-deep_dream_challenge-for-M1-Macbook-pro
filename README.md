# Customized-deep_dream_challenge-for-M1-Macbook-pro
Customized Deep Dream Challenge code by @SIrajology for M1 mac 
How To Install TensorFlow on M1 Mac (The Easy Way) based on https://caffeinedev.medium.com/how-to-install-tensorflow-on-m1-mac-8e9b91d93706
open terminal and paste  following instructions: 
1-       /bin/bash -c “$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
2-       xcode-select --install
then install Install miniforge for arm64 (Apple Silicon) by followin steps:
 1-       download miniforge3-MacOSX-arm64 from https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-arm64.sh
 2-       On macOS, you can install miniforge with Homebrew by running
          brew install miniforge
 After the installation of miniforge, by default, it gives us one base environment. You can turn off the default base env by running
  1-       conda config --set auto_activate_base false
  2-       Create a virtual environment:
              conda create --name mlp python=3.8
  3-       Activate virtual environment by running:
              conda activate mlp
Installing Tensorflow-MacOS:
  1-       Install the Tensorflow dependencies:
               conda install -c apple tensorflow-deps
  2-       Install base TensorFlow:
               pip install tensorflow-macos
  then you can run
            python M1DeepDream.py
           
