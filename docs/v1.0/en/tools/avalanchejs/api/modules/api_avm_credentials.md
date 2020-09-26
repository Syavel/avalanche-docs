[avalanche](../README.md) › [API-AVM-Credentials](api_avm_credentials.md)

# Module: API-AVM-Credentials

## Index

### Classes

* [NFTCredential](../classes/api_avm_credentials.nftcredential.md)
* [SECPCredential](../classes/api_avm_credentials.secpcredential.md)

### Functions

* [SelectCredentialClass](api_avm_credentials.md#const-selectcredentialclass)

## Functions

### `Const` SelectCredentialClass

▸ **SelectCredentialClass**(`credid`: number, ...`args`: Array‹any›): *[Credential](../classes/common_signature.credential.md)*

*Defined in [src/apis/avm/credentials.ts:23](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/apis/avm/credentials.ts#L23)*

Takes a buffer representing the credential and returns the proper [Credential](../classes/common_signature.credential.md) instance.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`credid` | number | A number representing the credential ID parsed prior to the bytes passed in  |
`...args` | Array‹any› | - |

**Returns:** *[Credential](../classes/common_signature.credential.md)*

An instance of an [Credential](../classes/common_signature.credential.md)-extended class.
