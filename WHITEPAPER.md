# PlaneSight Whitepaper

## Experimental Research into Steganography, Digital Value, and Media-Linked Ownership

**Version:** Experimental v0.9.1  
**Author:** Christian Blaze  
**License:** MIT License

---

# Abstract

PlaneSight is an experimental open-source research platform investigating the intersection of steganography, digital media, cryptography, and digital value.

The project began as a proof-of-concept exploring whether a Bitcoin private key could be embedded into an image and later recovered. This initial concept evolved into a broader research initiative focused on understanding how information can be concealed, preserved, and redundantly encoded across multiple forms of digital media.

PlaneSight explores techniques designed to survive transformations such as JPEG compression, resizing, format conversion, filtering, and metadata manipulation while simultaneously investigating whether media itself can become a carrier of cryptographic value.

This document describes the motivation, architecture, research goals, experimental methods, and future directions of the project.

---

# Introduction

Digital media can be copied infinitely at virtually zero cost.

Images, audio, video, and documents can be duplicated without degradation, creating challenges for scarcity, ownership, and preservation.

At the same time, cryptographic systems such as Bitcoin enable digital value to exist independently of centralized authorities.

PlaneSight explores the possibility of connecting these two worlds.

The central question is:

> Can digital media directly contain cryptographic value?

The project does not attempt to answer this question definitively. Instead, it provides a platform for experimentation and research.

---

# Origins of the Project

PlaneSight originated from a simple thought experiment.

A Bitcoin wallet could be created and funded. The private key controlling that wallet could then be encoded into an image using steganographic techniques.

Whoever successfully recovered the key would gain access to the associated bitcoin.

This concept immediately revealed several interesting challenges:

- How can hidden information survive image transformations?
- How much information can be concealed?
- How can hidden information remain visually undetectable?
- Can multiple independent encoding methods be combined?
- Can media become a bearer instrument for value?

These questions became the foundation of PlaneSight.

---

# Project Goals

The project has several primary goals.

## Goal 1: Steganography Research

Investigate practical methods for embedding information inside media while minimizing detection.

## Goal 2: Transformation Resilience

Study whether hidden information can survive:

- JPEG compression
- Resizing
- Scaling
- Filtering
- Format conversion
- Metadata stripping

## Goal 3: Multi-Layer Encoding

Explore whether the same payload can be redundantly encoded using multiple independent techniques simultaneously.

## Goal 4: Media-Linked Value

Investigate mechanisms through which digital media may carry cryptographic value.

---

# Current Architecture

PlaneSight currently functions as a steganography research framework rather than a single encoding algorithm.

The system supports experimentation with multiple encoding approaches.

Current research methods include:

- PNG Stealth
- JPEG Resilient
- Resize Lab
- Scale Lab
- DCT Lab
- Wavelet Lab
- Watermark Lab
- Metadata Embedding

Multiple methods may be combined simultaneously to evaluate compatibility and resilience.

---

# Multi-Layer Encoding

Traditional steganography often relies upon a single hiding mechanism.

PlaneSight explores a different model.

The same encrypted payload may be encoded simultaneously into:

- Pixel values
- Frequency coefficients
- Metadata
- Watermark structures
- Future audio channels
- Future video channels

Redundancy may increase the likelihood of successful recovery after transformations.

Future versions may automatically determine optimal encoding combinations based upon desired resilience objectives.

---

# Bitcoin-Backed Media

One area of investigation involves linking digital media with Bitcoin value.

A conceptual workflow might be:

1. Create a Bitcoin wallet.
2. Fund the wallet.
3. Encrypt the private key.
4. Encode the encrypted payload into media.
5. Distribute the media.

Possession of the media may provide a path toward recovering the associated value.

This remains an experimental concept and should not be interpreted as secure Bitcoin custody.

---

# Multisignature Media Rights Management

PlaneSight also explores the possibility of combining media distribution with multisignature Bitcoin wallets.

In a conceptual model:

- One signing key is embedded inside the media.
- Another signing key is controlled by the issuer or distributor.

Possession of the media alone would not immediately unlock the associated bitcoin.

Instead, the distributor could participate in signing transactions under predefined conditions.

Possible examples include:

- Time-locked redemption
- Vesting schedules
- Long-term holding incentives
- Ownership verification systems
- Collector reward programs

For example:

A media issuer may agree to release the full embedded value only after five years.

If redemption occurs earlier, only a portion of the value might be released.

Such mechanisms could incentivize preservation rather than redistribution.

These concepts remain theoretical and are intended as research topics rather than product specifications.

---

# Future Audio and Video Research

Current PlaneSight research focuses primarily on images.

Future development may explore:

## Audio Embedding

Encoding encrypted payloads into:

- Frequency bands
- Phase information
- Spread-spectrum audio signals

## Video Embedding

Encoding payloads into:

- Video frames
- Motion vectors
- Frequency-domain coefficients
- Metadata structures

## Cross-Media Redundancy

The same encrypted payload could potentially exist simultaneously within:

- Images
- Audio
- Video
- Metadata

creating multiple independent recovery paths.

---

# Security Considerations

PlaneSight is experimental.

No encoding method currently implemented should be considered secure storage for:

- Bitcoin
- Private keys
- Passwords
- Sensitive communications
- Valuable secrets

Known limitations include:

- Detection risk
- Data corruption
- Compression damage
- Transformation loss
- Implementation bugs
- Incomplete testing

Users should assume hidden information may be destroyed, detected, or become unrecoverable.

---

# Research Philosophy

PlaneSight is not simply a steganography project.

It is an exploration of whether media can become more than content.

The project investigates whether information, ownership, value, and media may become interconnected through cryptographic systems and resilient information encoding techniques.

The long-term vision is not merely to hide information.

The long-term vision is to explore whether digital media can evolve into a new class of value-bearing digital artifact.

---

# Disclaimer

PlaneSight is a research project.

Nothing described in this document should be interpreted as financial advice, security advice, or a recommendation to store meaningful amounts of Bitcoin using the software.

The project is experimental and provided for educational and research purposes only.

---

# License

PlaneSight is released under the MIT License.

See the LICENSE file for details.

---

*Proof-of-concept created by Christian Blaze.*
