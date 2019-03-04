# Installation

## Rust

https://www.rust-lang.org/tools/install

```sh
curl https://sh.rustup.rs -sSf | sh
```

=> Configuring the PATH environment variable:
```sh
➜  __RUST__ head ~/.zshrc
# Path to your oh-my-zsh installation.
export ZSH="/home/latty/.oh-my-zsh"

# RUST
export PATH="$HOME/.cargo/bin:$PATH"
```

## EvCxR Jupyter Kernel

https://github.com/google/evcxr/tree/master/evcxr_jupyter

```sh
sudo apt install libzmq3-dev jupyter-notebook
cargo install evcxr_jupyter
evcxr_jupyter --install
```

# Running

Just launching jupyter-notebook server:
```sh
➜  __RUST__ jupyter-notebook
[I 17:16:27.158 NotebookApp] Serving notebooks from local directory: /home/latty/Prog/__RUST__
[I 17:16:27.158 NotebookApp] The Jupyter Notebook is running at:
[I 17:16:27.158 NotebookApp] http://localhost:8888/?token=
[I 17:16:27.159 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[C 17:16:27.184 NotebookApp]

    To access the notebook, open this file in a browser:
        file:///home/latty/.local/share/jupyter/runtime/nbserver-7906-open.html
    Or copy and paste one of these URLs:
        http://localhost:8888/?token=
```

A new kernel 'Rust' is available !

![](./datas/jupyter_kernel_rust.png?raw=true "Rust Kernel in Jupyter Notebook")