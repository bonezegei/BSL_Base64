# BSL_Base64

**BSL_Base64** is a base64 encoding and decoding library designed for the **Bonezegei Scripting Language (BSL)**. It provides a simple, object-oriented approach to easily encode standard text strings into base64 format and decode base64 strings back into readable text within your `.bzg` scripts.

## Table of Contents
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Code Examples](#code-examples)
  - [1. Base64 Decode and Encode](#1-base64-decode-and-encode)
- [API Reference](#api-reference)
- [License & Author](#license--author)
- [Citation](#citation)

## Installation

Install `BSL_Base64` using the BSL Package Manager (`bzg`):

```bash
bzg install base64
```

## Getting Started

To use the library in your script, include the base64 module after installation and instantiate the object:

```javascript
include("lib/base64.bzg");

var base64 = base64();
```

## Code Examples

### 1. Base64 Decode and Encode

This example demonstrates how to instantiate the base64 object, encode a standard text string, and then decode it back to its original form.

```javascript
/*
    Base64 Example Decode and Encode
    Author: Jofel Batutay (Bonezegei)
    Date: August 29, 2026
*/

// include the library after Installation (" bzg install base64 ")
include("lib/base64.bzg");

var base64 = base64();

// var en = base64.encode("Bonezegei Scripting Language Base64 Library", true); //param 2 will treat param 1 as hex string 
var en = base64.encode("Bonezegei Scripting Language Base64 Library"); 
var de = base64.decode(en);

print("Encoded: " + en);
print("Decoded: " + de);
```

---

## API Reference

| Function / Method Signature | Return Value | Description |
| :--- | :--- | :--- |
| `base64()` | `Object` | Factory constructor that initializes and returns a new base64 object with attached native methods. |
| `base64.encode(text)` | `string` / `null` | Encodes the provided standard text string into a base64 formatted string. Returns `null` on failure. |
| `base64.decode(base64_string)` | `string` / `null` | Decodes the provided base64 string back into standard text. Returns `null` on invalid base64 input or failure. |

---

## License & Author

* **Author:** Jofel Batutay ([Bonezegei](https://github.com/bonezegei))
* **Date:** August 29, 2026
* **Website:** [bonezegei.com](https://bonezegei.com)

## Citation 
[![DOI](https://zenodo.org/badge/1350674211.svg)](https://doi.org/10.5281/zenodo.22163356)

If you use this library, please cite it as below:

**APA Format:**

Batutay, J. (2026). *bonezegei/BSL_Base64* [Computer software]. https://doi.org/10.5281/zenodo.22163356
