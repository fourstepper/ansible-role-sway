# ansible-molecule-submodule

This project is intended to be used as a testing base in multiple other ansible-related projects, imported as a submodule.

A requirements file can be placed in the root of the project into which this submodule is imported:

**A .molecule-converge.yml file is required, in a similar fashion.**

```
molecule
├── default
│   ├── converge.yml
│   ├── molecule.yml
│   └── verify.yml
.molecule-requirements.yml
.molecule-converge.yml
```

The molecule driver is podman.

The image for molecule is to be specified in the IMAGE environment variable, for example:

```
$ export IMAGE=geerlingguy/docker-fedora33-ansible
$ molecule test
```
