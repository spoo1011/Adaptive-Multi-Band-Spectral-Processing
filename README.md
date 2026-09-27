# Adaptive Multi-Band Spectral Processing for Audio Enhancement in Video Streams

## Overview

This project implements a MATLAB-based digital signal processing (DSP)
technique for reducing background noise from the audio track of a video.

The system extracts the audio from an input video and processes it in the
time-frequency domain using Short-Time Fourier Transform (STFT),
harmonic-percussive separation, spectral gating, and Butterworth filtering.

The enhanced audio is then merged with the original video to generate an
enhanced output video.

## Objectives

- Extract audio from a video.
- Analyze the audio in the time-frequency domain.
- Perform harmonic-percussive separation.
- Suppress unwanted background noise.
- Apply spectral gating for noise reduction.
- Preserve the main speech frequency range.
- Reconstruct the enhanced audio.
- Merge the enhanced audio with the original video.

## Processing Pipeline

```text
Input Video
     |
     v
Audio Extraction
     |
     v
Stereo to Mono Conversion
     |
     v
STFT Analysis
     |
     v
Harmonic/Percussive Separation
     |
     v
Harmonic Mask Generation
     |
     v
Spectral Gating
     |
     v
Speech Band Filtering
     |
     v
Audio Normalization
     |
     v
Enhanced Audio
     |
     v
Video Reconstruction
     |
     v
Audio-Video Merging
     |
     v
Enhanced Video
