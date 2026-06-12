# PlaneSight

## Languages

- 🇺🇸 English (this document)
- 🇪🇸 [Español](docs/es/README.md)

---

**PlaneSight** is an experimental open-source steganography research platform focused on hiding information inside digital media while exploring resilience against image transformations such as JPEG compression, resizing, filtering, and format conversion.

Originally conceived as a proof-of-concept for embedding Bitcoin private keys inside images, PlaneSight has evolved into a research environment for testing multiple steganographic techniques and exploring new ways to associate digital value with digital media.

---

# Vision

The original inspiration for PlaneSight was a simple question:

> Can Bitcoin be hidden inside an image?

The idea was to create a Bitcoin wallet, fund it with bitcoin, and encode the wallet's private key into an image. Whoever possesses the image and can successfully recover the key would gain access to the bitcoin associated with that media.

Over time, this concept expanded beyond simple image steganography into a broader exploration of how digital media and digital value might be linked together.

Future versions may explore:

- Image-based key storage
- Video-based key storage
- Audio-based key storage
- Metadata-based storage
- Multi-layer redundant encoding
- Cryptographic key splitting
- Multisignature custody models
- Media-linked digital ownership systems

---

# Current Features

- PNG Stealth embedding
- JPEG Resilient embedding
- Resize resilience experiments
- Scale resilience experiments
- DCT (frequency-domain) experiments
- Wavelet-based experiments
- Watermark experiments
- Metadata embedding
- Multi-method layering
- Compatibility verification

---

# Research Goals

PlaneSight investigates several questions:

## Can hidden information survive media transformations?

Examples include:

- PNG → JPEG conversion
- Resizing
- Recompression
- Metadata stripping
- Image editing

## Can multiple steganographic methods be layered together?

PlaneSight supports experimentation with combining multiple methods simultaneously and verifying whether they interfere with each other.

## Can digital media carry embedded value?

One long-term research direction is the possibility of embedding cryptographic secrets into media in a way that creates incentives to preserve, store, and protect the original files.

---

# Future Research Directions

## Multi-Layer Encoding

Future versions may redundantly encode encrypted payloads into:

- Image pixels
- Frequency-domain coefficients
- Audio tracks
- Video frames
- Metadata
- Container structures

The same encrypted payload could exist in multiple locations simultaneously, increasing resilience against damage or modification.

## Bitcoin-Backed Media

One area of exploration is the possibility of associating Bitcoin value with digital media.

For example:

1. A wallet is created and funded.
2. The wallet's private key is encrypted.
3. The encrypted payload is embedded into the media.
4. Ownership of the media implies potential access to the embedded value.

This remains a research concept and should not be considered secure storage for meaningful amounts of Bitcoin.

## Multisignature Media Rights Management

Future research may explore multisignature wallet structures where:

- One signing key is embedded within the media.
- Another signing key is held by the distributor or issuer.

In such a model, possession of the media alone would not grant immediate access to the bitcoin.

The distributor could participate in signing transactions under predefined conditions.

Examples might include:

- Time-based release schedules
- Vesting periods
- Collector rewards
- Digital ownership verification
- Long-term holding incentives

A media file could potentially contain embedded value that increases based on how long the media is preserved before redemption.

For example, a distributor could agree to release the full bitcoin value only after a specified holding period (such as five years). Earlier redemption might release only a portion of the embedded value. Such mechanisms could incentivize long-term preservation of digital media and discourage casual copying or redistribution.

These concepts are experimental and intended to inspire discussion and future research.

---

# Important Disclaimer

PlaneSight is an experimental research project.

The software has not been audited and should not be relied upon for:

- Long-term secret storage
- Bitcoin custody
- Secure communications
- Protection of valuable assets

Always assume hidden information can be lost, corrupted, detected, or destroyed.

Do not store significant amounts of bitcoin using PlaneSight.

---

# Contributing

Contributions, experiments, research ideas, and pull requests are welcome.

Areas of interest include:

- Steganography
- Watermarking
- Image processing
- Signal processing
- JPEG and video codecs
- Cryptography
- Bitcoin-related applications
- Error correction systems
- Media preservation

---

# License

This project is released under the MIT License.

See the LICENSE file for details.

---

*Proof-of-concept created by Christian Blaze.*