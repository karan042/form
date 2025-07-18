---
id: FieldApi
title: FieldApi
---

<!-- DO NOT EDIT: this page is autogenerated from the type comments -->

# Class: FieldApi\<TParentData, TName, TData, TOnMount, TOnChange, TOnChangeAsync, TOnBlur, TOnBlurAsync, TOnSubmit, TOnSubmitAsync, TFormOnMount, TFormOnChange, TFormOnChangeAsync, TFormOnBlur, TFormOnBlurAsync, TFormOnSubmit, TFormOnSubmitAsync, TFormOnServer, TParentSubmitMeta\>

Defined in: [packages/form-core/src/FieldApi.ts:863](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L863)

A class representing the API for managing a form field.

Normally, you will not need to create a new `FieldApi` instance directly.
Instead, you will use a framework hook/function like `useField` or `createField`
to create a new instance for you that uses your framework's reactivity model.
However, if you need to create a new instance manually, you can do so by calling
the `new FieldApi` constructor.

## Type Parameters

• **TParentData**

• **TName** *extends* [`DeepKeys`](../../type-aliases/deepkeys.md)\<`TParentData`\>

• **TData** *extends* [`DeepValue`](../../type-aliases/deepvalue.md)\<`TParentData`, `TName`\>

• **TOnMount** *extends* `undefined` \| `FieldValidateOrFn`\<`TParentData`, `TName`, `TData`\>

• **TOnChange** *extends* `undefined` \| `FieldValidateOrFn`\<`TParentData`, `TName`, `TData`\>

• **TOnChangeAsync** *extends* `undefined` \| `FieldAsyncValidateOrFn`\<`TParentData`, `TName`, `TData`\>

• **TOnBlur** *extends* `undefined` \| `FieldValidateOrFn`\<`TParentData`, `TName`, `TData`\>

• **TOnBlurAsync** *extends* `undefined` \| `FieldAsyncValidateOrFn`\<`TParentData`, `TName`, `TData`\>

• **TOnSubmit** *extends* `undefined` \| `FieldValidateOrFn`\<`TParentData`, `TName`, `TData`\>

• **TOnSubmitAsync** *extends* `undefined` \| `FieldAsyncValidateOrFn`\<`TParentData`, `TName`, `TData`\>

• **TFormOnMount** *extends* `undefined` \| `FormValidateOrFn`\<`TParentData`\>

• **TFormOnChange** *extends* `undefined` \| `FormValidateOrFn`\<`TParentData`\>

• **TFormOnChangeAsync** *extends* `undefined` \| `FormAsyncValidateOrFn`\<`TParentData`\>

• **TFormOnBlur** *extends* `undefined` \| `FormValidateOrFn`\<`TParentData`\>

• **TFormOnBlurAsync** *extends* `undefined` \| `FormAsyncValidateOrFn`\<`TParentData`\>

• **TFormOnSubmit** *extends* `undefined` \| `FormValidateOrFn`\<`TParentData`\>

• **TFormOnSubmitAsync** *extends* `undefined` \| `FormAsyncValidateOrFn`\<`TParentData`\>

• **TFormOnServer** *extends* `undefined` \| `FormAsyncValidateOrFn`\<`TParentData`\>

• **TParentSubmitMeta**

## Constructors

### new FieldApi()

```ts
new FieldApi<TParentData, TName, TData, TOnMount, TOnChange, TOnChangeAsync, TOnBlur, TOnBlurAsync, TOnSubmit, TOnSubmitAsync, TFormOnMount, TFormOnChange, TFormOnChangeAsync, TFormOnBlur, TFormOnBlurAsync, TFormOnSubmit, TFormOnSubmitAsync, TFormOnServer, TParentSubmitMeta>(opts): FieldApi<TParentData, TName, TData, TOnMount, TOnChange, TOnChangeAsync, TOnBlur, TOnBlurAsync, TOnSubmit, TOnSubmitAsync, TFormOnMount, TFormOnChange, TFormOnChangeAsync, TFormOnBlur, TFormOnBlurAsync, TFormOnSubmit, TFormOnSubmitAsync, TFormOnServer, TParentSubmitMeta>
```

Defined in: [packages/form-core/src/FieldApi.ts:995](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L995)

Initializes a new `FieldApi` instance.

#### Parameters

##### opts

[`FieldApiOptions`](../../interfaces/fieldapioptions.md)\<`TParentData`, `TName`, `TData`, `TOnMount`, `TOnChange`, `TOnChangeAsync`, `TOnBlur`, `TOnBlurAsync`, `TOnSubmit`, `TOnSubmitAsync`, `TFormOnMount`, `TFormOnChange`, `TFormOnChangeAsync`, `TFormOnBlur`, `TFormOnBlurAsync`, `TFormOnSubmit`, `TFormOnSubmitAsync`, `TFormOnServer`, `TParentSubmitMeta`\>

#### Returns

[`FieldApi`](../fieldapi.md)\<`TParentData`, `TName`, `TData`, `TOnMount`, `TOnChange`, `TOnChangeAsync`, `TOnBlur`, `TOnBlurAsync`, `TOnSubmit`, `TOnSubmitAsync`, `TFormOnMount`, `TFormOnChange`, `TFormOnChangeAsync`, `TFormOnBlur`, `TFormOnBlurAsync`, `TFormOnSubmit`, `TFormOnSubmitAsync`, `TFormOnServer`, `TParentSubmitMeta`\>

## Properties

### form

```ts
form: FormApi<TParentData, TFormOnMount, TFormOnChange, TFormOnChangeAsync, TFormOnBlur, TFormOnBlurAsync, TFormOnSubmit, TFormOnSubmitAsync, TFormOnServer, TParentSubmitMeta>;
```

Defined in: [packages/form-core/src/FieldApi.ts:907](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L907)

A reference to the form API instance.

***

### name

```ts
name: DeepKeys<TParentData>;
```

Defined in: [packages/form-core/src/FieldApi.ts:931](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L931)

The field name.

***

### options

```ts
options: FieldApiOptions<TParentData, TName, TData, TOnMount, TOnChange, TOnChangeAsync, TOnBlur, TOnBlurAsync, TOnSubmit, TOnSubmitAsync, TFormOnMount, TFormOnChange, TFormOnChangeAsync, TFormOnBlur, TFormOnBlurAsync, TFormOnSubmit, TFormOnSubmitAsync, TFormOnServer, TParentSubmitMeta>;
```

Defined in: [packages/form-core/src/FieldApi.ts:935](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L935)

The field options.

***

### store

```ts
store: Derived<FieldState<TParentData, TName, TData, TOnMount, TOnChange, TOnChangeAsync, TOnBlur, TOnBlurAsync, TOnSubmit, TOnSubmitAsync, TFormOnMount, TFormOnChange, TFormOnChangeAsync, TFormOnBlur, TFormOnBlurAsync, TFormOnSubmit, TFormOnSubmitAsync>>;
```

Defined in: [packages/form-core/src/FieldApi.ts:959](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L959)

The field state store.

***

### timeoutIds

```ts
timeoutIds: object;
```

Defined in: [packages/form-core/src/FieldApi.ts:986](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L986)

#### formListeners

```ts
formListeners: Record<ListenerCause, null | Timeout>;
```

#### listeners

```ts
listeners: Record<ListenerCause, null | Timeout>;
```

#### validations

```ts
validations: Record<ValidationCause, null | Timeout>;
```

## Accessors

### state

#### Get Signature

```ts
get state(): FieldState<TParentData, TName, TData, TOnMount, TOnChange, TOnChangeAsync, TOnBlur, TOnBlurAsync, TOnSubmit, TOnSubmitAsync, TFormOnMount, TFormOnChange, TFormOnChangeAsync, TFormOnBlur, TFormOnBlurAsync, TFormOnSubmit, TFormOnSubmitAsync>
```

Defined in: [packages/form-core/src/FieldApi.ts:983](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L983)

The current field state.

##### Returns

[`FieldState`](../../type-aliases/fieldstate.md)\<`TParentData`, `TName`, `TData`, `TOnMount`, `TOnChange`, `TOnChangeAsync`, `TOnBlur`, `TOnBlurAsync`, `TOnSubmit`, `TOnSubmitAsync`, `TFormOnMount`, `TFormOnChange`, `TFormOnChangeAsync`, `TFormOnBlur`, `TFormOnBlurAsync`, `TFormOnSubmit`, `TFormOnSubmitAsync`\>

## Methods

### clearValues()

```ts
clearValues(opts?): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1319](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1319)

Clear all values from the array.

#### Parameters

##### opts?

`UpdateMetaOptions`

#### Returns

`void`

***

### getInfo()

```ts
getInfo(): FieldInfo<TParentData>
```

Defined in: [packages/form-core/src/FieldApi.ts:1249](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1249)

Gets the field information object.

#### Returns

[`FieldInfo`](../../type-aliases/fieldinfo.md)\<`TParentData`\>

***

### getMeta()

```ts
getMeta(): FieldMeta<TParentData, TName, TData, TOnMount, TOnChange, TOnChangeAsync, TOnBlur, TOnBlurAsync, TOnSubmit, TOnSubmitAsync, TFormOnMount, TFormOnChange, TFormOnChangeAsync, TFormOnBlur, TFormOnBlurAsync, TFormOnSubmit, TFormOnSubmitAsync>
```

Defined in: [packages/form-core/src/FieldApi.ts:1217](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1217)

#### Returns

[`FieldMeta`](../../type-aliases/fieldmeta.md)\<`TParentData`, `TName`, `TData`, `TOnMount`, `TOnChange`, `TOnChangeAsync`, `TOnBlur`, `TOnBlurAsync`, `TOnSubmit`, `TOnSubmitAsync`, `TFormOnMount`, `TFormOnChange`, `TFormOnChangeAsync`, `TFormOnBlur`, `TFormOnBlurAsync`, `TFormOnSubmit`, `TFormOnSubmitAsync`\>

***

### ~~getValue()~~

```ts
getValue(): TData
```

Defined in: [packages/form-core/src/FieldApi.ts:1202](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1202)

Gets the current field value.

#### Returns

`TData`

#### Deprecated

Use `field.state.value` instead.

***

### handleBlur()

```ts
handleBlur(): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1670](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1670)

Handles the blur event.

#### Returns

`void`

***

### handleChange()

```ts
handleChange(updater): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1663](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1663)

Handles the change event.

#### Parameters

##### updater

[`Updater`](../../type-aliases/updater.md)\<`TData`\>

#### Returns

`void`

***

### insertValue()

```ts
insertValue(
   index, 
   value, 
   opts?): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1266](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1266)

Inserts a value at the specified index, shifting the subsequent values to the right.

#### Parameters

##### index

`number`

##### value

`TData` *extends* `any`[] ? `TData`\<`TData`\>\[`number`\] : `never`

##### opts?

`UpdateMetaOptions`

#### Returns

`void`

***

### mount()

```ts
mount(): () => void
```

Defined in: [packages/form-core/src/FieldApi.ts:1092](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1092)

Mounts the field instance to the form.

#### Returns

`Function`

##### Returns

`void`

***

### moveValue()

```ts
moveValue(
   aIndex, 
   bIndex, 
   opts?): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1310](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1310)

Moves the value at the first specified index to the second specified index.

#### Parameters

##### aIndex

`number`

##### bIndex

`number`

##### opts?

`UpdateMetaOptions`

#### Returns

`void`

***

### parseValueWithSchema()

```ts
parseValueWithSchema(schema): 
  | undefined
  | StandardSchemaV1Issue[]
```

Defined in: [packages/form-core/src/FieldApi.ts:1711](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1711)

Parses the field's value with the given schema and returns
issues (if any). This method does NOT set any internal errors.

#### Parameters

##### schema

[`StandardSchemaV1`](../../type-aliases/standardschemav1.md)\<`TData`, `unknown`\>

The standard schema to parse this field's value with.

#### Returns

  \| `undefined`
  \| [`StandardSchemaV1Issue`](../../interfaces/standardschemav1issue.md)[]

***

### parseValueWithSchemaAsync()

```ts
parseValueWithSchemaAsync(schema): Promise<
  | undefined
| StandardSchemaV1Issue[]>
```

Defined in: [packages/form-core/src/FieldApi.ts:1723](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1723)

Parses the field's value with the given schema and returns
issues (if any). This method does NOT set any internal errors.

#### Parameters

##### schema

[`StandardSchemaV1`](../../type-aliases/standardschemav1.md)\<`TData`, `unknown`\>

The standard schema to parse this field's value with.

#### Returns

`Promise`\<
  \| `undefined`
  \| [`StandardSchemaV1Issue`](../../interfaces/standardschemav1issue.md)[]\>

***

### pushValue()

```ts
pushValue(value, opts?): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1254](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1254)

Pushes a new value to the field.

#### Parameters

##### value

`TData` *extends* `any`[] ? `TData`\<`TData`\>\[`number`\] : `never`

##### opts?

`UpdateMetaOptions`

#### Returns

`void`

***

### removeValue()

```ts
removeValue(index, opts?): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1292](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1292)

Removes a value at the specified index.

#### Parameters

##### index

`number`

##### opts?

`UpdateMetaOptions`

#### Returns

`void`

***

### replaceValue()

```ts
replaceValue(
   index, 
   value, 
   opts?): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1279](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1279)

Replaces a value at the specified index.

#### Parameters

##### index

`number`

##### value

`TData` *extends* `any`[] ? `TData`\<`TData`\>\[`number`\] : `never`

##### opts?

`UpdateMetaOptions`

#### Returns

`void`

***

### setErrorMap()

```ts
setErrorMap(errorMap): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1686](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1686)

Updates the field's errorMap

#### Parameters

##### errorMap

`ValidationErrorMap`\<[`UnwrapFieldValidateOrFn`](../../type-aliases/unwrapfieldvalidateorfn.md)\<`TName`, `TOnMount`, `TFormOnMount`\>, [`UnwrapFieldValidateOrFn`](../../type-aliases/unwrapfieldvalidateorfn.md)\<`TName`, `TOnChange`, `TFormOnChange`\>, [`UnwrapFieldAsyncValidateOrFn`](../../type-aliases/unwrapfieldasyncvalidateorfn.md)\<`TName`, `TOnChangeAsync`, `TFormOnChangeAsync`\>, [`UnwrapFieldValidateOrFn`](../../type-aliases/unwrapfieldvalidateorfn.md)\<`TName`, `TOnBlur`, `TFormOnBlur`\>, [`UnwrapFieldAsyncValidateOrFn`](../../type-aliases/unwrapfieldasyncvalidateorfn.md)\<`TName`, `TOnBlurAsync`, `TFormOnBlurAsync`\>, [`UnwrapFieldValidateOrFn`](../../type-aliases/unwrapfieldvalidateorfn.md)\<`TName`, `TOnSubmit`, `TFormOnSubmit`\>, [`UnwrapFieldAsyncValidateOrFn`](../../type-aliases/unwrapfieldasyncvalidateorfn.md)\<`TName`, `TOnSubmitAsync`, `TFormOnSubmitAsync`\>\>

#### Returns

`void`

***

### setMeta()

```ts
setMeta(updater): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1222](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1222)

Sets the field metadata.

#### Parameters

##### updater

[`Updater`](../../type-aliases/updater.md)\<[`FieldMetaBase`](../../type-aliases/fieldmetabase.md)\<`TParentData`, `TName`, `TData`, `TOnMount`, `TOnChange`, `TOnChangeAsync`, `TOnBlur`, `TOnBlurAsync`, `TOnSubmit`, `TOnSubmitAsync`, `TFormOnMount`, `TFormOnChange`, `TFormOnChangeAsync`, `TFormOnBlur`, `TFormOnBlurAsync`, `TFormOnSubmit`, `TFormOnSubmitAsync`\>\>

#### Returns

`void`

***

### setValue()

```ts
setValue(updater, options?): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1209](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1209)

Sets the field value and run the `change` validator.

#### Parameters

##### updater

[`Updater`](../../type-aliases/updater.md)\<`TData`\>

##### options?

`UpdateMetaOptions`

#### Returns

`void`

***

### swapValues()

```ts
swapValues(
   aIndex, 
   bIndex, 
   opts?): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1301](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1301)

Swaps the values at the specified indices.

#### Parameters

##### aIndex

`number`

##### bIndex

`number`

##### opts?

`UpdateMetaOptions`

#### Returns

`void`

***

### update()

```ts
update(opts): void
```

Defined in: [packages/form-core/src/FieldApi.ts:1145](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1145)

Updates the field instance with new options.

#### Parameters

##### opts

[`FieldApiOptions`](../../interfaces/fieldapioptions.md)\<`TParentData`, `TName`, `TData`, `TOnMount`, `TOnChange`, `TOnChangeAsync`, `TOnBlur`, `TOnBlurAsync`, `TOnSubmit`, `TOnSubmitAsync`, `TFormOnMount`, `TFormOnChange`, `TFormOnChangeAsync`, `TFormOnBlur`, `TFormOnBlurAsync`, `TFormOnSubmit`, `TFormOnSubmitAsync`, `TFormOnServer`, `TParentSubmitMeta`\>

#### Returns

`void`

***

### validate()

```ts
validate(cause, opts?): unknown[] | Promise<unknown[]>
```

Defined in: [packages/form-core/src/FieldApi.ts:1630](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L1630)

Validates the field value.

#### Parameters

##### cause

`ValidationCause`

##### opts?

###### skipFormValidation?

`boolean`

#### Returns

`unknown`[] \| `Promise`\<`unknown`[]\>
