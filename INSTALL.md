**Installation**

First, use your package manager (`brew` if you're using macOS) to install [FontForge](http://fontforge.github.io/en-US/).

Then, clone the repo, build and install:

```bash
git clone git@github.com:powerline/fontpatcher.git
cd fontpatcher
./setup.py build
./setup.py install
```

**Usage**:

```
powerline-fontpatcher [-h] [--no-rename] [--source-font font]
                             font [font ...]

Font patcher for Powerline. Requires FontForge with Python bindings. Stores
the patched font as a new, renamed font file by default.

positional arguments:
  font                font files to patch

optional arguments:
  -h, --help          show this help message and exit
  --no-rename         don't add " for Powerline" to the font name
  --source-font font  source symbol font
```

**Tip:**

`powerline-fontpatcher` tries to find `powerline-symbold.sfd` in `/usr/share/...` by default. If this fails, then try:

1. Copying the font you'd like to patch into the `fontpatcher` directory.

2. Specifying `--source-font` like so:

`powerline-patcher --source-font ./fonts/powerline-symbols.sfd ./SomeFont.otf`


