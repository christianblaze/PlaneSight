# PlaneSight

**Proof-of-concept steganography tool created by Christian Blaze**

PlaneSight is a browser-based steganography tool that allows users to hide text messages inside digital images and later recover them from the encoded image.

The project combines spread-spectrum embedding techniques with Reed-Solomon error correction to improve robustness against image degradation and JPEG recompression.

All processing takes place locally in the browser. Images and messages are never uploaded to a server.

---

## Features

- Hide text messages inside images
- Recover hidden messages from encoded images
- Browser-based, no installation required
- Reed-Solomon error correction
- Spread-spectrum redundancy
- JPEG survivability testing
- Offline operation

---

## How It Works

PlaneSight embeds data into image luminance values using a spread-spectrum approach. Each bit of information is distributed across multiple pixels, while Reed-Solomon error correction helps recover the original message if the image experiences compression or minor modifications.

The goal is to create a more resilient form of steganography than simple least-significant-bit (LSB) encoding.

---

## Usage

### Encode

1. Open PlaneSight in your browser.
2. Upload an image.
3. Enter a secret message.
4. Click **Encode & Download**.
5. Save the generated PNG image.

### Decode

1. Open PlaneSight in your browser.
2. Upload an encoded image.
3. Click **Extract Message**.
4. Read the recovered message.

---

## Inspiration

PlaneSight originated from an exploration of whether Bitcoin private keys could be embedded inside digital media.

The initial idea was simple: create a Bitcoin wallet, fund it with bitcoin, and encode the wallet's private key into an image. In this model, the image itself becomes a carrier of value, allowing information and economic value to travel together.

While the current project focuses on steganography rather than Bitcoin integration, that original question inspired the development of PlaneSight and continues to influence its long-term direction.

For more information about the broader vision of the project, see:

**[VISION.md](VISION.md)**

---

## Disclaimer

PlaneSight is an experimental proof-of-concept and has not undergone formal security review, cryptographic audit, or independent testing.

The software should not currently be relied upon for protecting sensitive information, storing Bitcoin private keys, or securing valuable assets.

This project is intended for research, educational, and experimental purposes.

---

## Contributing

Contributions, experiments, bug reports, and ideas are welcome.

If you are interested in steganography, cryptography, Bitcoin, image processing, or digital ownership systems, feel free to open an issue or submit a pull request.

---

## License

MIT License

Proof-of-concept created by Christian Blaze.
