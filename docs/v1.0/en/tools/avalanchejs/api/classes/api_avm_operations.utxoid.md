[avalanche](../README.md) › [API-AVM-Operations](../modules/api_avm_operations.md) › [UTXOID](api_avm_operations.utxoid.md)

# Class: UTXOID

Class for representing a UTXOID used in [[TransferableOp]] types

## Hierarchy

* [NBytes](common_nbytes.nbytes.md)

  ↳ **UTXOID**

## Index

### Constructors

* [constructor](api_avm_operations.utxoid.md#constructor)

### Properties

* [bsize](api_avm_operations.utxoid.md#protected-bsize)
* [bytes](api_avm_operations.utxoid.md#protected-bytes)

### Methods

* [clone](api_avm_operations.utxoid.md#clone)
* [create](api_avm_operations.utxoid.md#create)
* [fromBuffer](api_avm_operations.utxoid.md#frombuffer)
* [fromString](api_avm_operations.utxoid.md#fromstring)
* [getSize](api_avm_operations.utxoid.md#getsize)
* [toBuffer](api_avm_operations.utxoid.md#tobuffer)
* [toString](api_avm_operations.utxoid.md#tostring)
* [comparator](api_avm_operations.utxoid.md#static-comparator)

## Constructors

###  constructor

\+ **new UTXOID**(): *[UTXOID](api_avm_operations.utxoid.md)*

*Overrides [NBytes](common_nbytes.nbytes.md).[constructor](common_nbytes.nbytes.md#constructor)*

*Defined in [src/apis/avm/ops.ts:555](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/apis/avm/ops.ts#L555)*

Class for representing a UTXOID used in [[TransferableOp]] types

**Returns:** *[UTXOID](api_avm_operations.utxoid.md)*

## Properties

### `Protected` bsize

• **bsize**: *number*

*Inherited from [NBytes](common_nbytes.nbytes.md).[bsize](common_nbytes.nbytes.md#protected-bsize)*

*Defined in [src/common/nbytes.ts:25](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/common/nbytes.ts#L25)*

___

### `Protected` bytes

• **bytes**: *Buffer*

*Inherited from [NBytes](common_nbytes.nbytes.md).[bytes](common_nbytes.nbytes.md#protected-bytes)*

*Defined in [src/common/nbytes.ts:23](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/common/nbytes.ts#L23)*

## Methods

###  clone

▸ **clone**(): *this*

*Overrides [NBytes](common_nbytes.nbytes.md).[clone](common_nbytes.nbytes.md#abstract-clone)*

*Defined in [src/apis/avm/ops.ts:547](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/apis/avm/ops.ts#L547)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [NBytes](common_nbytes.nbytes.md).[create](common_nbytes.nbytes.md#abstract-create)*

*Defined in [src/apis/avm/ops.ts:553](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/apis/avm/ops.ts#L553)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  fromBuffer

▸ **fromBuffer**(`buff`: Buffer, `offset`: number): *number*

*Inherited from [NBytes](common_nbytes.nbytes.md).[fromBuffer](common_nbytes.nbytes.md#frombuffer)*

*Defined in [src/common/nbytes.ts:56](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/common/nbytes.ts#L56)*

Takes a [[Buffer]], verifies its length, and stores it.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`buff` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

The size of the [Buffer](https://github.com/feross/buffer)

___

###  fromString

▸ **fromString**(`utxoid`: string): *number*

*Overrides [NBytes](common_nbytes.nbytes.md).[fromString](common_nbytes.nbytes.md#fromstring)*

*Defined in [src/apis/avm/ops.ts:528](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/apis/avm/ops.ts#L528)*

Takes a base-58 string containing an [UTXOID](api_avm_operations.utxoid.md), parses it, populates the class, and returns the length of the UTXOID in bytes.

**Parameters:**

Name | Type |
------ | ------ |
`utxoid` | string |

**Returns:** *number*

The length of the raw [UTXOID](api_avm_operations.utxoid.md)

___

###  getSize

▸ **getSize**(): *number*

*Inherited from [NBytes](common_nbytes.nbytes.md).[getSize](common_nbytes.nbytes.md#getsize)*

*Defined in [src/common/nbytes.ts:32](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/common/nbytes.ts#L32)*

Returns the length of the [Buffer](https://github.com/feross/buffer).

**Returns:** *number*

The exact length requirement of this class

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [NBytes](common_nbytes.nbytes.md).[toBuffer](common_nbytes.nbytes.md#tobuffer)*

*Defined in [src/common/nbytes.ts:76](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/common/nbytes.ts#L76)*

**Returns:** *Buffer*

A reference to the stored [Buffer](https://github.com/feross/buffer)

___

###  toString

▸ **toString**(): *string*

*Overrides [NBytes](common_nbytes.nbytes.md).[toString](common_nbytes.nbytes.md#tostring)*

*Defined in [src/apis/avm/ops.ts:517](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/apis/avm/ops.ts#L517)*

Returns a base-58 representation of the [UTXOID](api_avm_operations.utxoid.md).

**Returns:** *string*

___

### `Static` comparator

▸ **comparator**(): *function*

*Defined in [src/apis/avm/ops.ts:511](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/apis/avm/ops.ts#L511)*

Returns a function used to sort an array of [UTXOID](api_avm_operations.utxoid.md)s

**Returns:** *function*

▸ (`a`: [UTXOID](api_avm_operations.utxoid.md), `b`: [UTXOID](api_avm_operations.utxoid.md)): *0 | 1 | -1*

**Parameters:**

Name | Type |
------ | ------ |
`a` | [UTXOID](api_avm_operations.utxoid.md) |
`b` | [UTXOID](api_avm_operations.utxoid.md) |
