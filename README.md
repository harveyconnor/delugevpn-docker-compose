# delugevpn-docker-compose

## Installation
1. Copy the .env.example file to .env and edit the values inside to match your setup.
```
cp .env.example .env
```
2. Make sure you edit the .env file with the correct `IP` and `DOWNLOADS_DIR` 
3. Wherever you set your `DOWNLOADS_DIR`, make sure the following folders are in there:
- complete
- incomplete

## Usage
```
docker-compose up -d
```
Once it is running (check with `docker ps` and `docker-compose logs deluge`), you need to set your download directories in the web client at http://`IP`:8112. Set the directories to:

Downloads: `/data/incomplete`
Downloads complete: `/data/complete`

For more information on the environment variables. Please check the [binhex/arch-delugevpn](https://hub.docker.com/r/binhex/arch-delugevpn/) docker hub or github page.

## Contributors
- [@binhex](https://github.com/binhex)
- [@harveyconnor](https://github.com/harveyconnor)
