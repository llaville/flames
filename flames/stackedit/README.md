# Enable and Configure StackEdit

This section will guide you through getting StackEdit integrated into the Devilbox.

**See also**

* [Docker Hub: StackEdit](https://hub.docker.com/r/benweet/stackedit)
* [StackEdit GitHub Project](https://github.com/benweet/stackedit)
    
## Overview

### StackEdit settings

In case of StackEdit, the file is `flames/stackedit/docker-compose.override.yml`. This file
must be copied into the root of the Devilbox git directory.

| What        | How and where |
| ----------- | ------------- |
| Example compose file  | `flames/stackedit/docker-compose.override.yml` | 

**StackEdit**

| What        | How and where |
| ----------- | ------------- |
| Container IP address  | `̀172.16.238.181`                         |
| Container name        | `stackedit`                              |
| Exposed port          | `8181` (can be changed via `.env`)       | 
| Available at          | `http://localhost:8181`                  |


### StackEdit env variables

Additionally the following `.env` variables can be created for easy configuration:

| Variable                        | Default value | Description                                                    |
| ------------------------------- | ------------- | -------------------------------------------------------------- |
| `HOST_PORT_STACKEDIT`           | `8181`        | Controls the host port on which StackEdit will be available at. |
| `STACKEDIT_SERVER`              | `latest`      | Controls the StackEdit version to use.                          |
