[avalanche](../README.md) › [Utils-Payload](../modules/utils_payload.md) › [UTF8Payload](utils_payload.utf8payload.md)

# Class: UTF8Payload

Class for payloads representing UTF8 encoding.

## Hierarchy

* [PayloadBase](utils_payload.payloadbase.md)

  ↳ **UTF8Payload**

  ↳ [SVGPayload](utils_payload.svgpayload.md)

  ↳ [CSVPayload](utils_payload.csvpayload.md)

  ↳ [YAMLPayload](utils_payload.yamlpayload.md)

  ↳ [EMAILPayload](utils_payload.emailpayload.md)

  ↳ [URLPayload](utils_payload.urlpayload.md)

  ↳ [ONIONPayload](utils_payload.onionpayload.md)

  ↳ [MAGNETPayload](utils_payload.magnetpayload.md)

## Index

### Constructors

* [constructor](utils_payload.utf8payload.md#constructor)

### Properties

* [payload](utils_payload.utf8payload.md#protected-payload)
* [typeid](utils_payload.utf8payload.md#protected-typeid)

### Methods

* [fromBuffer](utils_payload.utf8payload.md#frombuffer)
* [getContent](utils_payload.utf8payload.md#getcontent)
* [getPayload](utils_payload.utf8payload.md#getpayload)
* [returnType](utils_payload.utf8payload.md#returntype)
* [toBuffer](utils_payload.utf8payload.md#tobuffer)
* [typeID](utils_payload.utf8payload.md#typeid)
* [typeName](utils_payload.utf8payload.md#typename)

## Constructors

###  constructor

\+ **new UTF8Payload**(`payload`: any): *[UTF8Payload](utils_payload.utf8payload.md)*

*Overrides [PayloadBase](utils_payload.payloadbase.md).[constructor](utils_payload.payloadbase.md#constructor)*

*Defined in [src/utils/payload.ts:272](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L272)*

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`payload` | any | undefined | Buffer utf8 string  |

**Returns:** *[UTF8Payload](utils_payload.utf8payload.md)*

## Properties

### `Protected` payload

• **payload**: *Buffer* = Buffer.alloc(0)

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[payload](utils_payload.payloadbase.md#protected-payload)*

*Defined in [src/utils/payload.ts:168](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L168)*

___

### `Protected` typeid

• **typeid**: *number* = 1

*Overrides [PayloadBase](utils_payload.payloadbase.md).[typeid](utils_payload.payloadbase.md#protected-typeid)*

*Defined in [src/utils/payload.ts:265](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L265)*

## Methods

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[fromBuffer](utils_payload.payloadbase.md#frombuffer)*

*Defined in [src/utils/payload.ts:206](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L206)*

Decodes the payload as a [Buffer](https://github.com/feross/buffer) including 4 bytes for the length and TypeID.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getContent

▸ **getContent**(): *Buffer*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[getContent](utils_payload.payloadbase.md#getcontent)*

*Defined in [src/utils/payload.ts:188](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L188)*

Returns the payload content (minus typeID).

**Returns:** *Buffer*

___

###  getPayload

▸ **getPayload**(): *Buffer*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[getPayload](utils_payload.payloadbase.md#getpayload)*

*Defined in [src/utils/payload.ts:196](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L196)*

Returns the payload (with typeID).

**Returns:** *Buffer*

___

###  returnType

▸ **returnType**(): *string*

*Overrides [PayloadBase](utils_payload.payloadbase.md).[returnType](utils_payload.payloadbase.md#abstract-returntype)*

*Defined in [src/utils/payload.ts:270](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L270)*

Returns a string for the payload.

**Returns:** *string*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[toBuffer](utils_payload.payloadbase.md#tobuffer)*

*Defined in [src/utils/payload.ts:219](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L219)*

Encodes the payload as a [Buffer](https://github.com/feross/buffer) including 4 bytes for the length and TypeID.

**Returns:** *Buffer*

___

###  typeID

▸ **typeID**(): *number*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[typeID](utils_payload.payloadbase.md#typeid)*

*Defined in [src/utils/payload.ts:174](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L174)*

Returns the TypeID for the payload.

**Returns:** *number*

___

###  typeName

▸ **typeName**(): *string*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[typeName](utils_payload.payloadbase.md#typename)*

*Defined in [src/utils/payload.ts:181](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/payload.ts#L181)*

Returns the string name for the payload's type.

**Returns:** *string*
