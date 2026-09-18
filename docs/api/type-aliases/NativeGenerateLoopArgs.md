[**NeuroLink API Reference**](../README.md)

---

[NeuroLink API Reference](../README.md) / NativeGenerateLoopArgs

# Type Alias: NativeGenerateLoopArgs

> **NativeGenerateLoopArgs** = `object`

Defined in: [types/generate.ts:1801](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1801)

Inputs to the shared native generate loop (`core/nativeGenerateLoop.ts`).
One loop serves every provider whose delegating model exposes a v3-shaped
`doGenerate`; the provider supplies the wire details.

## Properties

### doGenerate

> **doGenerate**: (`options`) => `Promise`\<`Record`\<`string`, `unknown`\>\>

Defined in: [types/generate.ts:1802](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1802)

#### Parameters

##### options

`Record`\<`string`, `unknown`\>

#### Returns

`Promise`\<`Record`\<`string`, `unknown`\>\>

---

### conversation

> **conversation**: `Record`\<`string`, `unknown`\>[]

Defined in: [types/generate.ts:1806](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1806)

Conversation in the message-builder shape each doGenerate converts itself.

---

### tools?

> `optional` **tools?**: `Record`\<`string`, `unknown`\>[]

Defined in: [types/generate.ts:1808](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1808)

Tool declarations in the v3 shape doGenerate already knows how to convert.

---

### toolsRecord

> **toolsRecord**: `Record`\<`string`, `unknown`\>

Defined in: [types/generate.ts:1810](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1810)

Registered tools, used to execute a call the model asks for.

---

### toolChoice?

> `optional` **toolChoice?**: `unknown`

Defined in: [types/generate.ts:1811](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1811)

---

### responseFormat?

> `optional` **responseFormat?**: `Record`\<`string`, `unknown`\>

Defined in: [types/generate.ts:1812](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1812)

---

### providerOptions?

> `optional` **providerOptions?**: `Record`\<`string`, `Record`\<`string`, `unknown`\>\>

Defined in: [types/generate.ts:1813](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1813)

---

### maxSteps

> **maxSteps**: `number`

Defined in: [types/generate.ts:1814](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1814)

---

### maxOutputTokens?

> `optional` **maxOutputTokens?**: `number`

Defined in: [types/generate.ts:1815](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1815)

---

### temperature?

> `optional` **temperature?**: `number`

Defined in: [types/generate.ts:1816](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1816)

---

### abortSignal?

> `optional` **abortSignal?**: `AbortSignal`

Defined in: [types/generate.ts:1817](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1817)

---

### toolTimeoutMs?

> `optional` **toolTimeoutMs?**: `number` \| `null`

Defined in: [types/generate.ts:1819](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1819)

Per-tool-execution cap, forwarded into `guardToolExecutor`. `null` for no bound.

---

### runStep

> **runStep**: (`call`) => `Promise`\<`Record`\<`string`, `unknown`\>\>

Defined in: [types/generate.ts:1821](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1821)

Wraps one step: retry ladder plus provider error classification.

#### Parameters

##### call

() => `Promise`\<`Record`\<`string`, `unknown`\>\>

#### Returns

`Promise`\<`Record`\<`string`, `unknown`\>\>
