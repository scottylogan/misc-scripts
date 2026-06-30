# Miscellaneous Scripts

## Password and Passphrase Scripts

### `passphrase` _[options]_

Generate a passphrase.

| Option | Description                    |
|--------|--------------------------------|
| -h     | show usage / help and defaults |
| -m N   | set minimum word length        |
| -M N   | set maximum word length        |
| -n N   | set number of words            |
| -s C   | set word separator             |

### `pwgen` _[options]_

Generate a password.

| Option | Description                          |
|--------|--------------------------------------|
| -c     | include capital / upper case letters |
| -n     | include numbers / digits             |
| -y     | include punctuation                  |
| -a     | equivalent to `-c -n -y`             |

## Other Scripts

### `yubikey`

Update SSH Agent to use / not use the PKCS11 provider for Yubikey. Run
`yubikey` after inserting or removing a Yubikey containing an SSH
keypair. It will prompt for PIN / touch as required.

### `marked` _file.md_

Open a file with the [Marked](https://marked2app.com/) Markdown previewer

### `git-touch`

Recursively set the timestamps on all the files in the local directory
to their last commit date / time.

### `capturepages`

Capture all page title and URLs from Chrome as Markdown, using [chrome://inspect#pages]
