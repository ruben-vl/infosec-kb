# Encoding

## Useful Links

- Rot13 encode/decode: https://rot13.com/
- Cipher Identifier and Analyzer: https://www.boxentriq.com/code-breaking/cipher-identifier

## Base64

Encode

```bash
echo string | base64
```

Decode

```bash
echo encoded_string | base64 -d
```

## Hex

Encode

```bash
echo string | xxd -p
```

Decode

```bash
echo encoded_string | xxd -p -r
```

## Rot13

Encode

```bash
echo string | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

Decoding is exactly the same as encoding.
Can also be done through an online tool: https://rot13.com/