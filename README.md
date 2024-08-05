# Introduction

[COSMIC Terminal](https://github.com/pop-os/cosmic-term) is a terminal emulator for COSMIC. When I used it, I noticed that with the default theme, i.e., Cosmic Dark, my [pywal](https://github.com/dylanaraps/pywal) colors were messed up.

To solve this I manually copied and pasted colors 0-7 and respective foreground and cursor color from the `colors.sh` file at `~/.cache/wal/colors.sh`.

# How to use

- First, copy this repo:
```bash
git clone https://github.com/dharmik2319/pywal-cosmic-term.git
```

- Then, after `cd`ing into the directory, install the dependencies.
```bash
pip install -r requirements.txt
```

- Now the script is ready for use:
```bash
python main.py
```

That's it. For advanced usage run with `-h` flag. You can output to a custom file [Default: `./pywal.ron`], use your own sample file [Default: `./COSMIC Dark.ron`], and give the path to your pywal colors file [Default: `~/.cache/wal/colors`].

# Acknowledgement

- [`Pyron`](https://github.com/cswinter/pyron/) or [`python-ron`](https://pypi.org/project/python-ron/) made the task a bit easier.
