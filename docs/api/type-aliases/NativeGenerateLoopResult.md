[**NeuroLink API Reference**](../README.md)

---

[NeuroLink API Reference](../README.md) / NativeGenerateLoopResult

# Type Alias: NativeGenerateLoopResult

> **NativeGenerateLoopResult** = `object`

Defined in: [types/generate.ts:1826](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1826)

## Properties

### text

> **text**: `string`

Defined in: [types/generate.ts:1827](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1827)

---

### reasoning?

> `optional` **reasoning?**: `string`

Defined in: [types/generate.ts:1829](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1829)

Joined reasoning content parts from the final step, when the vendor sent any.

---

### finishReason

> **finishReason**: `string`

Defined in: [types/generate.ts:1830](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1830)

---

### rawFinishReason?

> `optional` **rawFinishReason?**: `string`

Defined in: [types/generate.ts:1831](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1831)

---

### inputTokens

> **inputTokens**: `number`

Defined in: [types/generate.ts:1832](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1832)

---

### outputTokens

> **outputTokens**: `number`

Defined in: [types/generate.ts:1833](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1833)

---

### cacheReadTokens

> **cacheReadTokens**: `number`

Defined in: [types/generate.ts:1834](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1834)

---

### cacheWriteTokens

> **cacheWriteTokens**: `number`

Defined in: [types/generate.ts:1835](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1835)

---

### toolsUsed

> **toolsUsed**: `string`[]

Defined in: [types/generate.ts:1836](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1836)

---

### steps

> **steps**: `number`

Defined in: [types/generate.ts:1837](https://github.com/juspay/neurolink/blob/release/src/lib/types/generate.ts#L1837)
