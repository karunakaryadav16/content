---
title: EncodedVideoChunk.timestamp
slug: Web/API/EncodedVideoChunk/timestamp
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.EncodedVideoChunk.timestamp
---

{{APIRef("WebCodecs API")}}{{SeeCompatTable}}

The **`timestamp`** read-only property of the {{domxref("EncodedVideoChunk")}} interface returns an integer indicating the timestamp of the video in microseconds.

## Value

An integer.

## Examples

In the following example the `timestamp` is printed to the console.

```js
const init = {
  type: "key",
  data: videoBuffer,
  timestamp: 23000000,
  duration: 2000000,
};
chunk = EncodedVideoChunk(init);
console.log(chunk.timestamp); //23000000
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
