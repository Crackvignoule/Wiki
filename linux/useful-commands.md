# Useful Commands

#### Change default shell:

```bash
chsh -s /bin/bash $USER
```

#### Restart shell (for bash, zsh, may not work with fish, csh, sh...)

<pre><code>exec "$SHELL" <a data-footnote-ref href="#user-content-fn-1">-l</a>
</code></pre>

#### **Create GIF with your screen view:**

```bash
sudo apt install -y peek && peek
```

#### **fuck :** [_**The Fuck**_](https://github.com/nvbn/thefuck) **is a magnificent app that corrects errors in previous console commands. Install script:**

```bash
#!/usr/bin/env bash
sudo apt update
sudo apt install python3-dev python3-pip python3-setuptools python3-venv
python3 -m venv ~/.config/thefuck
source ~/.config/thefuck/bin/activate
pip install setuptools
pip install git+https://github.com/nvbn/thefuck.git
echo 'export PATH="$HOME/.config/thefuck/bin:$PATH"' >> ~/.bashrc
fuck
fuck
```

#### Remove unused packages

```bash
sudo apt autoremove
```

[^1]: login shell: it will reload \~/.bashrc ...
