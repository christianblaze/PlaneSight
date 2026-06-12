# PlaneSight Methods

PlaneSight is an experimental steganography research platform that explores multiple techniques for embedding information into digital media.

Different methods have different tradeoffs between:

- Capacity
- Invisibility
- JPEG resilience
- Resize resilience
- Computational complexity
- Recovery reliability

This document provides a high-level overview of each method currently implemented or under investigation.

---

# PNG Stealth

PNG Stealth focuses on visually subtle embedding.

The goal is to make changes difficult for a human observer to notice while maintaining reliable recovery from the original PNG file.

## Advantages

- High capacity
- Minimal visible artifacts
- Fast encoding and decoding

## Limitations

- Fragile to JPEG conversion
- Fragile to resizing
- Fragile to filtering and editing

---

# JPEG Resilient

JPEG Resilient focuses on surviving JPEG recompression.

Instead of relying solely on exact pixel values, the method introduces stronger image modifications that can survive moderate JPEG quality reduction.

## Advantages

- Better JPEG survival
- Reliable recovery under moderate compression

## Limitations

- Lower capacity
- More visible modifications
- Not designed for aggressive resizing

---

# Resize Lab

Resize Lab is an experimental system intended to investigate whether hidden information can survive image scaling operations.

The method uses normalized regions rather than absolute pixel locations.

## Advantages

- Potential resilience to proportional resizing
- Supports redundancy experiments

## Limitations

- Experimental
- Limited capacity
- Can introduce visible artifacts
- Currently unreliable under aggressive resizing

---

# Scale Lab

Scale Lab explores alternative approaches to scale-invariant encoding.

The objective is to determine whether hidden information can be recovered after images are resized while maintaining visual quality.

## Advantages

- Potential future resize resilience
- Research platform for scale-invariant encoding

## Limitations

- Experimental
- Under active development

---

# DCT Lab

DCT (Discrete Cosine Transform) Lab explores frequency-domain embedding.

JPEG itself uses DCT compression internally, making this approach attractive for future JPEG-resistant steganography.

## Advantages

- Potential JPEG resilience
- Frequency-domain embedding

## Limitations

- Experimental
- Capacity limitations
- Requires additional synchronization techniques

---

# Wavelet Lab

Wavelet Lab explores embedding information into wavelet coefficients.

Wavelet-based techniques are commonly used in digital watermarking research.

## Advantages

- Multi-scale representation
- Potential robustness against transformations

## Limitations

- Experimental
- Performance and reliability still under investigation

---

# Watermark Lab

Watermark Lab explores lightweight watermarking techniques.

The goal is to introduce detectable patterns without significantly altering visual appearance.

## Advantages

- Lightweight
- Low computational cost

## Limitations

- Lower capacity
- Not intended for large payloads

---

# Metadata Embedding

Metadata embedding stores information inside image metadata rather than image pixels.

## Advantages

- High reliability while metadata remains intact
- No visual modifications

## Limitations

- Metadata can be stripped by:
  - Social networks
  - Image editors
  - Screenshots
  - Re-exports

---

# Multi-Layer Encoding

One of PlaneSight's primary research goals is the ability to encode the same payload across multiple independent methods simultaneously.

For example:

- Metadata
- Pixel-domain embedding
- Frequency-domain embedding
- Watermarking
- Future audio embedding
- Future video embedding

By storing the same encrypted payload in multiple locations, the system may achieve greater resilience against damage or transformation.

---

# Future Research

Future versions of PlaneSight may investigate:

- Audio steganography
- Video steganography
- Frequency-domain video encoding
- Multi-signature Bitcoin media systems
- Media-linked digital ownership
- Multi-layer cryptographic key storage
- Self-verifying media
- Distributed recovery systems

---

# Experimental Status

PlaneSight is a research project.

Methods described in this document should be considered experimental unless explicitly stated otherwise.

No method should currently be relied upon for secure storage of valuable secrets or Bitcoin.