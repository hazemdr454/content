---
title: "URLSearchParams: getAll() method"
short-title: getAll()
slug: Web/API/URLSearchParams/getAll
page-type: web-api-instance-method
browser-compat: api.URLSearchParams.getAll
---

{{ApiRef("URL API")}}

The **`getAll()`** method of the {{domxref("URLSearchParams")}}
interface returns all the values associated with a given search parameter as an array.

{{availableinworkers}}

## Syntax

```js-nolint
getAll(name)
```

### Parameters

- `name`
  - : The name of the parameter to return.

### Return value

An array of strings, which may be empty if no values for the given parameter are found.

## Examples

```js
let url = new URL("https://example.com?foo=1&bar=2");
let params = new URLSearchParams(url.search);

//Add a second foo parameter.
params.append("foo", 4);

console.log(params.getAll("foo")); //Prints ["1","4"].
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
