
Installation
------------

  Download:

```bash
git clone https://github.com/jack-nie/tmux-conf.git ~/.tmux
```

  Copy tmux config to home:

```bash
ln -s ~/.tmux/.tmux.conf ~/.tmux.conf
```

  Go to config dir:

```bash
cd ~/.tmux
```

Stats
-----

### tmux-mem-cpu-load

Works on Linux and OS X.

  Prep ourself to download submodule:

```bash
git submodule init
```

  Download submodule:

```bash
git submodule update
```

  Change dir to tmux-mem-cpu-load:

```bash
cd ~/.tmux/vendor/tmux-mem-cpu-load
```

  General make file:

```bash
cmake .
```

  Compile our binary:

```bash
make
```

  Install our binary to `/usr/local/bin/tmux-mem-cpu-load`:

```bash
sudo make install
```

  Go home:

```bash
cd ~
```

  Launch tmux:
```
tmux
```
  And press `Control + a` then `d` to go back to the terminal.

  Update config:

```bash
tmux source-file ~/.tmux.conf
```

### basic-cpu-and-memory.tmux

(Cross platform, tested with python 2.7+)

Update March 19, 2014. Works with psutil 2.0 now.

Install ``psutil``:

```bash
sudo pip install psutil
```

copy ``~/.tmux/vendor/basic-cpu-and-memory.tmux`` to bin:

```bash
sudo cp ~/.tmux/vendor/basic-cpu-and-memory.tmux /usr/local/bin/tmux-mem-cpu-load
```

make executable:
```bash
sudo chmod +x /usr/local/bin/tmux-mem-cpu-load
```

