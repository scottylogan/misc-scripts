# Miscellaneous Scripts

`ec2` is now part of `ec2-tools`, called `ec2-run`.

## LDAP Scripts

### accounts attribute=value [attrs]

Wrapper around an LDAP search for the Stanford Accounts tree.

### people attribute=value [attrs]

Wrapper around an LDAP search for the Stanford People tree.


## IT Lab Scripts

### bastion name

SSH to `bastion.${name}.stanford.edu`

### my-deb-s3

Wrapper around the `deb-s3` Ruby Gem to update the IT Lab APT repo
(http://repo.itlab.stanford.edu).

### mysql-itlab

Wrapper script to connect to the IT Lab MySQL server. This script requires a
`~/.mylogin.cnf` file (created with
[`mysql_config_editor`](https://dev.mysql.com/doc/refman/5.7/en/mysql-config-editor.html) containing a `itlab` login-path. Further customization is possible using the `[clientitlab]` section in `~/.my.cnf`; for example:

```
    [clientitlab]
    ssl-ca = /Users/swl/share/ssl/certs/rds-combined-ca-bundle.pem
    ssl-mode = VERIFY_IDENTITY
```

## Password and Passphrase Scripts

### passphrase

Generate a four word passphrase.

### pwgen

Generate a password.

|Option |Description|
|-------|-----------|
|-c     |Include capital / upper case letters|
|-n     |Include numbers / digits|
|-y     |Include punctuation|
|-a     |Equivalent to `-c -n -y`|


## Other Scripts

### yubikey

Update SSH Agent to use / not use the PKCS11 provider for Yubikey. Run
`yubikey` after inserting or removing a Yubikey containing an SSH
keypair. It will prompt for PIN / touch as required.

### marked
