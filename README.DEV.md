# Developer Guide Lines

## Directory Structure

```
sap-base-settings/
├── defaults
│   └── main.yml
├── files
├── handlers
│   └── main.yml
├── LICENSE
├── meta
│   └── main.yml
├── README.DEV.md
├── README.md
├── tasks
│   ├── configuration.yml
│   └── main.yml
├── templates
├── tests
│   ├── inventory
│   └── test.yml
└── vars
    └── main.yml

8 directories, 11 files
```

The deployment of this role follows the style guide from Adfinis Sygroup. [Click Here](https://docs.adfinis-sygroup.ch/public/ansible-guide/styling_guide.html) for more info

## Where/How to make change/additions

There are no required packages to install, so there is only a configuration.yml
This role is currently RHEL 7 only
