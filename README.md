[![Ansible Galaxy](https://ansible.l3d.space/svg/l3d.gopass.svg)](https://galaxy.ansible.com/l3d/gopass)
[![MIT License](https://ansible.l3d.space/svg/l3d.gopass_license.svg)](LICENSE)
[![Maintainance](https://ansible.l3d.space/svg/l3d.gopass_maintainance.svg)](https://ansible.l3d.space/#l3d.gopass)
# Gopass Ansible Rolle

Ansile role to install the Password Manager [gopass](https://www.gopass.pw/). Gopass is a simple but powerful password manager for your terminal. And it is 100% API Compatible to the standard unix password manager [pass](https://passwordstore.org).

This role will only install the gopass passwordmanager. You have to configure and edit it by yourself 😉

## Variables
| Name | Value | Function |
| ---- | ----- | -------- |
| ``gopass__add_apt_repo`` | ``true`` | Install Gopass keyring and apt list on debian based Systems |
| ``gopass__install_jsonapi`` | ``true`` | Install gopass-jsonapi integration for browser integration |
| ``gopass__install_haveibeenpwnd`` | ``true`` | Install haveibeenpwnd.com integration |
| ``gopass__install_git_credential`` | ``true`` | Install haveibeenpwnd.com integration |
| ``gopass__install_zbar_tools`` | ``true`` | Install optional zbar tooling to read qrcodes |
| ``submodules_versioncheck`` | ``false`` | Run optional versionscheck to prevent old versions of tis ansible |

## Requirements
The ``community.general`` collection is required for some parts of this ansible role.
You can install it with this command:
```bash
ansible-galaxy collection install -r requirements.yml --upgrade
```

## Contributing
Please feel free to open a issue. Or suggest changes and improvements via Pull-Request. I will be happy to have a look at it.
