# Install AWS VPN Client on Debian Bookworm

Installs `awsvpnclient` on Debian Bookworm and takes care of fixing all the issues
the package has.

## Install ansible

Run:

```sh
sudo apt install pipx
pipx install --include-deps ansible
pipx ensurepath
```

Restart your shell or do `source ~/.profile`.

## Run the playbook

```
./main.yml
```

Enter your sudo password (BECOME password). Let the playbook run. Once the
playbook is done running, you should have a working AWS VPN Client install.
