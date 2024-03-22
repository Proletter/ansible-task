## Configuration Management Task - Starter

Here you will find some starter code, and basic information on how to get started!

Notes:

1. Provide solution in `playbook.yml` file
2. Use the dependencies from `requirements.txt`
3. The targeted machine is Ubuntu 22.04 LTS - You should use molecule setup presented in `molecule` directory
4. Add any additional information to the README if you think it's needed

These molecule commands may come in handy:

Create clean container:

```bash
molecule create
```

Executes playbook on the container:

```bash
molecule converge
```

Remove the container:

```bash
molecule destroy
```

### How to run playbook
- Install ansible and all dependencies by running `pip3 install -r requirements.txt`
- Update the inventory.ini file with the IP address, user and path to ssh private key of the remote machine
- Run `ansible-playbook -i inventory.ini playbook.yaml`