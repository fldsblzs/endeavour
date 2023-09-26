# onedrive

- [Repository](https://github.com/abraunegg/onedrive/blob/master/README.md)
- [Usage](https://github.com/abraunegg/onedrive/blob/master/docs/USAGE.md)
- [Docker](https://github.com/abraunegg/onedrive/blob/master/docs/Docker.md)

## Manual setup with docker `run`

```sh
export ONEDRIVE_UID=`id -u`
export ONEDRIVE_GID=`id -g`
export ONEDRIVE_DATA_DIR="${HOME}/OneDrive"
export ONEDRIVE_CONFIG_DIR="${HOME}/Configuration/OneDrive"
mkdir -p ${ONEDRIVE_DATA_DIR}
docker run -it --name onedrive -v "${ONEDRIVE_CONFIG_DIR}:/onedrive/conf" \
    -v "${ONEDRIVE_DATA_DIR}:/onedrive/data" \
    -e "ONEDRIVE_UID=${ONEDRIVE_UID}" \
    -e "ONEDRIVE_GID=${ONEDRIVE_GID}" \
    driveone/onedrive:edge
```