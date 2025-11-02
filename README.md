<p align="center">
<img src="https://media1.tenor.com/m/CgCL3w8WgXkAAAAC/rias-gremory-highschool-dxd.gif" width=650/>
</p>

---
<p align="center">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=36&pause=1000&color=BC13FE&center=true&width=550&lines=make+-j%24(nproc);Source+based;Linux+Nerd;Compile+from+Source" alt="Typing SVG"/>
</p>

---
<p align="left">
<img src="https://media.tenor.com/NeJfHqkmdMIAAAAj/tux-linux-penguin.gif" width=230 />
</p>

# About me

**13-year-old Linux systems enthusiast & Dev bash**

> *I believe in tools that solve real problems with elegant solutions. Whether it's a Bash script or a kernel patch, if it makes the system better, it's worth building.*

---

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/simeulinuxkaliaiwr/simeulinuxkaliaiwr/output/pacman-contribution-graph-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/simeulinuxkaliaiwr/simeulinuxkaliaiwr/output/pacman-contribution-graph.svg">
  <img alt="pacman contribution graph" src="https://raw.githubusercontent.com/simeulinuxkaliaiwr/simeulinuxkaliaiwr/output/pacman-contribution-graph.svg">
</picture>

###
---

## 🚀 My Journey

* Linux user for 1.5 years - started with Mint, now running Gentoo as main OS with Arch Linux dual-boot

* Started programming in August of 2025

* Gentoo for development and learning

* Arch for gaming and testing new projects like clilog

* Hyprland on both systems because tiling WMs are life

---

## 🛠️ What I Do

* Build practical CLI tools (Bash, Python, Flask)

* Maintain **[clilog-git in AUR](https://www.aur.archlinux.org/packages/clilog-git)**

* Compile my own kernels

   > Break things and learn how to fix them

---

## Tools and Languages
<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="50" alt="Python"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bash/bash-original.svg" width="50" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="50" alt="Git"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/neovim/neovim-original.svg" width="50" />
  <img src="https://raw.githubusercontent.com/devicons/devicon/ca28c779441053191ff11710fe24a9e6c23690d6/icons/vim/vim-original.svg" width="50" alt="vim" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/archlinux/archlinux-original.svg" width="50" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" width="50" />
  <img src="https://www.gentoo.org/assets/img/logo/gentoo-signet.svg" width="50" />
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/C_Programming_Language.svg/1086px-C_Programming_Language.svg.png" width="45" />
</p>

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=simeulinuxkaliaiwr&layout=compact&theme=radical"/>
  <img src="https://github-readme-stats.vercel.app/api?username=simeulinuxkaliaiwr&show_icons=true&theme=radical"/>
</p>

---

<p align="center">
<img src="https://streak-stats.demolab.com?user=simeulinuxkaliaiwr&theme=radical"/>
</p>

---

### 🔧 Current Setup & Philosophy
```

# My GRUB command-line reflects my approach to systems
GRUB_CMDLINE_LINUX_DEFAULT="loglevel=3 quiet \
lsm=lockdown,yama,apparmor,bpf \
random.trust_cpu=0 \
slab_nomerge init_on_alloc=1 init_on_free=1 page_poison=1 \
pti=on spectre_v2=on spec_store_bypass_disable=on \
mds=full,nosmt tsx=off"

# Translation: Security-first, performance-tuned, no compromises.
```

---

### 🚀 Future goals & Systems Deep Dive

*My journey is about refinement. These are the core targets for the next 6-12 months, focusing on systems programming, kernel interaction, and mastering modern Linux standards.*

---

### 🌟 Current Projects
> **[`clilog`](https://www.github.com/simeulinuxkaliaiwr/clilog)**

* Minimalist CLI task manager with TUI and Web interface made in [python](python.org) with [flask](https://flask.palletsprojects.com/en/stable/). Built in bash because sometimes the old ways are the best ways.

> **Working on 2 new projects:** `pkgwhy` and `grrec`🚧

---

### What is `pkgwhy`?

pkgwhy (Why is this package here?) is a command-line utility (CLI), written in rust, whose main purpose is to act as a diagnostic and software tracing tool for Linux systems based on *[arch linux](https://www.archlinux.org)*, which uses pacman as package manager. (initially only for pacman, but later it will be ported to other package managers, such as dnf, apt, portage, etc.)

It aims to answer the fundamental question: Why is a particular package installed on the system?

Example of use:
```
$ pkgwhy neovim

→ Explicitly installed: 2024-03-15 (user: you)

→ Dependencies brought: 12 packages

→ Recent use: 4.2h/day (high)

$ pkgwhy lib32-glibc

→ Installed as a dependency of: steam (2024-02-10)

→ Never used directly
```

---

### What is `grrec`?

Grrec is a fast, C-based command-line screen recorder for Wayland, focused on providing superior user experience through simple presets and native integration.

*I am making grrec bc i don't like [wf-recorder](https://github.com/ammen99/wf-recorder) output.*

Example of use:
```
# Basic Usage - Records the current output (screen) with a default, balanced preset.
# The output file is automatically named (e.g., grrec-2025-10-11_21-18-50.mp4).
$ grrec

# Records a specific, visually selected area of the screen. 
# Uses a visual tool (like slurp) for selection before recording starts.
$ grrec --select

# Records the active window only, using a fast codec for web sharing.
$ grrec --active-window --preset web-share

# Records with a specific output file name, forcing 60 frames per second (FPS).
$ grrec -f my_gameplay.mkv --framerate 60

# Records the screen, including the system's audio input (e.g., speaker output or microphone).
$ grrec --with-audio

# Advanced Use: Uses a high-quality preset (e.g., AV1 or H.265) and a custom quality scale (0-100).
$ grrec --preset high-quality --quality 85 -f presentation.mp4
```

---

📫 Let's Connect

- Github: [simeulinuxkaliaiwr](https://www.github.com/simeulinuxkaliaiwr)
- AUR Account: [AUR Account](https://aur.archlinux.org/account/Guilherme_bash/)
- Tiktok: [Tiktok](https://www.tiktok.com/@gz.xt7n)
- **Email**: [Email account](mailto:leonsombrio244@gmail.com)

---
*Fun fact: I created my email when I was 8 years old. Some of us start early.*

---
*Made by [simeulinuxkaliaiwr](https://www.github.com/simeulinuxkaliaiwr) based on [Jox0101011](https://www.github.com/Jox0101011)*
