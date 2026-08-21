# debian-postinst
Here is a simple script to initialize your minimal Debian installation!
=======
# Debian Post-Install

A simple post-installation toolkit for minimal Debian systems.

This project automates the initial configuration of a fresh Debian installation by setting up APT repositories, installing common packages, and configuring a comfortable command-line environment.

## Features

* Support for **Debian Stable** and **Debian Testing**
* Configure APT repositories
* Includes repository presets

  * Official Debian
  * MobinHost
  * Shatel
* Configure shell environment

  * `.bashrc`
  * `.vimrc`
  * `.tmux.conf`
  * `.pythonrc`
* Automate common post-installation tasks
* Easy to customize and extend

## Project Structure

```text
.
├── debian-postinst.sh
├── environment
│   ├── .bashrc
│   ├── .pythonrc
│   ├── .tmux.conf
│   └── .vimrc
└── repositories
    ├── stable
    │   ├── china-tsinghua.sources
    │   ├── china-ustc.sources
    │   ├── iran-liara.sources
    │   ├── iran-mobinhost.sources
    │   ├── iran-shatel.sources
    │   ├── official-debian.sources
    │   └── russia-yandex.sources
    └── testing
        ├── china-tsinghua.sources
        ├── china-ustc.sources
        ├── iran-mobinhost.sources
        ├── iran-shatel.sources
        ├── official-debian.sources
        └── russia-yandex.sources
```

## Requirements

* Debian 12 (Bookworm) or newer
* Root privileges 
* Internet connection

## Installation

Clone the repository:

```bash
git clone https://github.com/morteza-j/debian-postinst.git
cd debian-postinst
```

Run the installer:

```bash
bash debian-postinst.sh
```

## Customization

* Repository configurations are located in the `repositories/` directory.
* Shell configuration files are stored in the `environment/` directory.
* Feel free to modify these files before running the installer to match your preferences.

## Disclaimer

This script modifies your APT repository configuration and user environment. Always review the source code before executing it, especially on production systems.

## Contributing

Issues, feature requests, and pull requests are welcome.

## License

GNU GENERAL PUBLIC LICENSE Version 3
