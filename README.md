# cdw<br>[![GitHub Actions][actions-img]][actions-url] [![Patreon][patreon-img]][patreon-url] [![PayPal][paypal-img]][paypal-url] [![Discord][discord-img]][discord-url]

cdw is a simple shell tool that allows you to cd into a Windows path directly in wsl.

## Download

* [GitHub Releases](https://github.com/justalemon/cdw/releases)
* [GitHub Actions](https://github.com/justalemon/cdw/actions) (experimental versions)

## Installation

Download and copy `cdw.sh` into your `/etc/profile.d` directory. If you are using Arch Linux, you can run makepkg -si to install it.

## Usage

After installation, log out and then log back in. Then, run the `cdw [path]` command to change the directory to a Windows directory. Please note that you might need to single or double quote the path due to backspaces.

[actions-img]: https://img.shields.io/github/actions/workflow/status/justalemon/cdw/main.yml?branch=master&label=actions
[actions-url]: https://github.com/justalemon/cdw/actions
[patreon-img]: https://img.shields.io/badge/support-patreon-FF424D.svg
[patreon-url]: https://www.patreon.com/lemonchan
[paypal-img]: https://img.shields.io/badge/support-paypal-0079C1.svg
[paypal-url]: https://paypal.me/justalemon
[discord-img]: https://img.shields.io/badge/discord-join-7289DA.svg
[discord-url]: https://discord.gg/Cf6sspj
