# nvidia-smi++
A tool for enriching the output of nvidia-smi.

# Additional features
When checking process information, you can get
- a **docker container name** instead of an username
- an **execution command** instead of a process name
- a colored output for better readability

# Install
`pip3 install nvidia-htop`

and copy nvidia-smi-plus.py into any directory you want. (recommend $HOME directory)

Then,
`chmod +x nvidia-smi-plus.py`

It will make the file executable.

Add an alias into your `~/.zshrc` or `~/.bashrc`

`alias nvidia-smi=$YOUR_DIRECTORY/nvidai-smi-plus.py`

If you want colored output,

`alias nvidia-smi=$YOUR_DIRECTORY/nvidai-smi-plus.py -c`

If you want output with commandline length,

`alias nvidia-smi=$YOUR_DIRECTORY/nvidai-smi-plus.py -l`

# Usage
Just run the following command:

```bash
nvidia-smi
```

:blush::blush::blush:

# Screenshot
![Screenshot](screen.png)

# Acknowledgments
This repo highly depends on https://github.com/peci1/nvidia-htop. Thanks for his nice work!
