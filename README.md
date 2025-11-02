# Miscellaneous Scripts

## Password and Passphrase Scripts

### `passphrase`

Generate a four word passphrase.

### `pwgen` _[options]_

Generate a password.

|Option |Description|
|-------|-----------|
|-c     |Include capital / upper case letters|
|-n     |Include numbers / digits|
|-y     |Include punctuation|
|-a     |Equivalent to `-c -n -y`|

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

## Stanford LDAP Scripts

### `su-ldap`

Wrapper around an LDAP search. Copy / symlink `su-ldap` to make shortcuts for specific trees:

* `accounts` - search the Stanford Accounts tree
* `ldapgroups` - search the Stanford Groups tree
* `people` - search the Stanford People tree

Usage: `script` _searchfilter_ _[attrs]_

