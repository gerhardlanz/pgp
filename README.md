# PGP Public Key

Key ID: `0x20B3B7B9DDC083D0`

Fingerprint: `967B D238 B445 0141 E971  ADB8 20B3 B7B9 DDC0 83D0`

## Retrieve key from Proton

```
curl https://mail-api.proton.me/pks/lookup?op=get&search=me@gerhardla.nz | gpg --import
```

## Retrieve key from keyserver

Locate key:
```
gpg --auto-key-locate keys.openpgp.org --locate-keys 20B3B7B9DDC083D0
```

Add key to keychain:
```
gpg --keyserver keys.openpgp.org --recv-keys 20B3B7B9DDC083D0
```

Display information for imported key:
```
gpg -k 20B3B7B9DDC083D0
```

Refresh all keys (e.g. new revocation certificates and subkeys):
```
gpg --refresh-keys
```

Remove key from keychain:
```
gpg --batch --yes --delete-keys 20B3B7B9DDC083D0
```
