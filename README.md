# Ramp Challenge - Base64 Decoder

## Overview
This challenge demonstrates Base64 decoding using JavaScript's `atob()` function to reveal encoded URLs and instructions.

## Problem Description
The Ramp challenge provides a Base64-encoded string that contains a URL with further challenge instructions. To access these instructions, the encoded string must be decoded using the `atob()` function.

## How Base64 Encoding Works

### What is Base64?
Base64 is an **encoding scheme** (not encryption) that converts binary data into ASCII text. It uses 64 printable characters: `A-Z`, `a-z`, `0-9`, `+`, and `/`.

### Key Characteristics:
- **Reversible**: Data can be encoded and decoded without loss
- **Text-safe**: Converts binary data to text that can be safely transmitted
- **Size increase**: Encoded data is ~33% larger than original
- **Not secure**: Base64 is encoding, not encryption - anyone can decode it

### Common Use Cases:
- Embedding binary data in JSON/XML
- Email attachments (MIME)
- Data URIs for images
- API authentication tokens
- URL obfuscation (like in this challenge)

## The `atob()` Function

### Syntax:
```javascript
const decoded = atob(encodedString)