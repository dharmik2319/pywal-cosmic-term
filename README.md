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

# Images for reference

- Before:
  ![screenshot-2024-08-05-11-29-19](https://github.com/user-attachments/assets/3dfb5583-ceaa-4d00-84be-0930404767d9)

- After:
  ![screenshot-2024-08-05-11-28-10](https://github.com/user-attachments/assets/5cf48bcf-4d74-4a9f-a069-17edc95fe7b9)

(The terminal and other Cosmic components themed with [cosmic_ext_bg_theme](https://github.com/wash2/cosmic_ext_bg_theme?tab=readme-ov-file#table-of-contents).)

# Acknowledgement

- [`Pyron`](https://github.com/cswinter/pyron/) or [`python-ron`](https://pypi.org/project/python-ron/) made the task a bit easier.
