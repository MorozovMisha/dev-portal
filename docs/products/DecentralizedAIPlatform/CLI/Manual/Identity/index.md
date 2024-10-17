# Identity

```sh
	usage: snet identity [-h] ACTION ... 
```

## actions

`ACTION`

    

Possible choices: list, create, delete, andrey

## Sub-commands

### list

List of identities

```sh
	snet identity list [-h] 
```

### create

Create a new identity

```sh
	snet identity create [-h] [--mnemonic MNEMONIC] [--private-key
PRIVATE_KEY] [--keystore-path KEYSTORE_PATH] [--network NETWORK] [--wallet-
index WALLET_INDEX] IDENTITY_NAME IDENTITY_TYPE 
```

#### Positional Arguments

`IDENTITY_NAME`

    

Name of identity to create

`IDENTITY_TYPE`

    

Possible choices: rpc, mnemonic, key, trezor, ledger, keystore

Type of identity to create from [‘rpc’, ‘mnemonic’, ‘key’, ‘trezor’, ‘ledger’,
‘keystore’]

#### Named Arguments

`--mnemonic`

    

BIP39 mnemonic for ‘mnemonic’ identity_type

`--private-key`

    

Hex-encoded private key for ‘key’ identity_type

`--keystore-path`

    

Path of the JSON encrypted file for ‘keystore’ identity_type

`--network`

    

Network this identity will be bind to (obligatory for ‘rpc’ identity_type,
optional for others)

`--wallet-index`

    

Default wallet index for this account (default is 0)

Default: `0`

### delete

Delete an identity

```sh
	snet identity delete [-h] IDENTITY_NAME 
```

#### Positional Arguments

`IDENTITY_NAME`

    

Possible choices: andrey

Name of identity to delete from [‘andrey’]

### andrey

Switch to andrey identity

```sh
	snet identity andrey [-h] 
```

