[avalanche](../README.md) › [API-AVM-Outputs](api_avm_outputs.md)

# Module: API-AVM-Outputs

## Index

### Classes

* [AmountOutput](../classes/api_avm_outputs.amountoutput.md)
* [NFTMintOutput](../classes/api_avm_outputs.nftmintoutput.md)
* [NFTOutput](../classes/api_avm_outputs.nftoutput.md)
* [NFTTransferOutput](../classes/api_avm_outputs.nfttransferoutput.md)
* [SECPMintOutput](../classes/api_avm_outputs.secpmintoutput.md)
* [SECPTransferOutput](../classes/api_avm_outputs.secptransferoutput.md)
* [TransferableOutput](../classes/api_avm_outputs.transferableoutput.md)

### Variables

* [bintools](api_avm_outputs.md#const-bintools)

### Functions

* [SelectOutputClass](api_avm_outputs.md#const-selectoutputclass)

## Variables

### `Const` bintools

• **bintools**: *[BinTools](../classes/utils_bintools.bintools.md)‹›* = BinTools.getInstance()

*Defined in [src/apis/avm/outputs.ts:11](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/apis/avm/outputs.ts#L11)*

## Functions

### `Const` SelectOutputClass

▸ **SelectOutputClass**(`outputid`: number, ...`args`: Array‹any›): *[Output](../classes/common_output.output.md)*

*Defined in [src/apis/avm/outputs.ts:20](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/apis/avm/outputs.ts#L20)*

Takes a buffer representing the output and returns the proper Output instance.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`outputid` | number | A number representing the inputID parsed prior to the bytes passed in  |
`...args` | Array‹any› | - |

**Returns:** *[Output](../classes/common_output.output.md)*

An instance of an [Output](../classes/common_output.output.md)-extended class.
