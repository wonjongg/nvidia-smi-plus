# nvidia-smi++
A tool for enriching the output of nvidia-smi.

## Additional features
When checking process information, you can get
- a **docker container name** instead of an username
- an **execution command** instead of a process name
- a colored output for better readability

**Notes:** why do you want to check docker container name instead of an username?

If nvidia-docker users do not specify their username when executing their docker containers, usernames of processes are always 'root' by default. So, the username information isn't informative. Instead, I visualize a nvidia-docker container name to check who is running a process.

## Install
`pip3 install nvidia-htop`

and copy nvidia-smi-plus.py into any directory you want. (recommend $HOME directory)

Then,
`chmod +x nvidia-smi-plus.py`

It will make the file executable.

Add an alias into your `~/.zshrc` or `~/.bashrc`

`alias nvidia-smi='$YOUR_DIRECTORY/nvidia-smi-plus.py'`

If you want colored output,

`alias nvidia-smi='$YOUR_DIRECTORY/nvidia-smi-plus.py -c'`

If you want output with commandline length,

`alias nvidia-smi='$YOUR_DIRECTORY/nvidia-smi-plus.py -l'`

## Usage
Just run the following command:

```bash
nvidia-smi
```

:blush::blush::blush:

## Screenshot
![Screenshot](screen.png)

## Acknowledgements
This repo highly depends on https://github.com/peci1/nvidia-htop. Thanks for his nice work!
