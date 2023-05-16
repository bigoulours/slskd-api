# slskd-api

## Goal
This project aims at providing a python API for [slskd](https://github.com/slskd/slskd).

A comprehensive python API could help improve integration and increase slskd adoption by enabling rapid development of various software, like:
 * Desktop/Mobile Clients
 * [beets](https://github.com/beetbox/beets) plugin(s)
 * [headphones](https://github.com/rembo10/headphones) integration

## Installation
For the moment, please install manually:
```
pip install .
```

## Usage
Create a `slskd` instance with the following:
```
import slskd_api
slskd = slskd_api.SlskdClient(host, api_key, url_base)
```
Then you'll be able to access all API methods, like:
```
app_status = slskd.application.state()
available_rooms = slskd.rooms.get_all()
```
See the [doc](https://slskd-api.readthedocs.io/) for further details.
