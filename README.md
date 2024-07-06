# Pebble Codespace

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/blockarchitech/pebble-codespace)

A GitHub Codespace for easy development of Pebble apps.

## Usage guide

Simply press the button above and create a new codespace. GitHub should walk you through the steps of creating a codespace. **Note: It does take a while to build (~200 seconds). Please be patient.**

To login (and use --cloudpebble as a connection with the pebble tool), use the following steps:
- Run `pebble login`.
- Click "open" to open the Rebble authorization page, and press authorize.
- You will be redirected to a localhost:60000 page, where your web browser will complain.
- Go back to your codespace, click ports, and copy the link for port 60000. Replace the localhost:60000 in the URL with your copied link, keeping the query parameter (?code=...)
- You are now logged in. Try to install or get logs from a phone with developer connection enabled using `--cloudpebble`

## C IntelliSense

The include paths are already added for you if you installed the 'C/C++ Dev Kit" extension reccomended by the codespace. VSCode might complain that it can't find `message_keys.auto.h`, but run `pebble build` and this should go away.

## Emulator

This is currently being worked on. It is not supported as of now. 