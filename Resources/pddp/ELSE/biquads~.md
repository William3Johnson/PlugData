---
title: biquads~

description: Biquad Series

categories:
 - object

pdcategory: Audio Filters

inlets:
  1st:
  - type: signal
    description: the signal to be filtered
  - type: list
    description: list of biquad coefficients
  - type: clear
    description: clears the filter's memory
  - type: bypass <float>
    description: <1> bypasses the input, <0> turns the filter on
  
outlets:
  1st:
  - type: signal
    description: the filtered signal

draft: false
---

[biquads~] is a series of biquad filters in cascade. Each biquad section is defined as a list of 5 coefficients (in the same way as Pd Vanilla's [biquad~]). Below we have a series of two biquad sections in cascade. The maximum number of filter stages is 50, which provides up to 100th order filters.