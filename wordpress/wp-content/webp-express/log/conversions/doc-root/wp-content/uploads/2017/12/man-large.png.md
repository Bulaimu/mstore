WebP Express 0.17.2. Conversion triggered using bulk conversion, 2019-10-12 08:57:28

*WebP Convert 2.3.0*  ignited.
- PHP version: 7.0.33
- Server software: Apache

Stack converter ignited

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2017/12/man-large.png
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/12/man-large.png.webp
- log-call-arguments: true
- converters: (array of 9 items)

The following options have not been explicitly set, so using the following defaults:
- converter-options: (empty array)
- shuffle: false
- preferred-converters: (empty array)
- extra-converters: (empty array)

The following options were supplied and are passed on to the converters in the stack:
- alpha-quality: 80
- encoding: "auto"
- metadata: "none"
- near-lossless: 60
- quality: 85
------------


*Trying: cwebp* 

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2017/12/man-large.png
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/12/man-large.png.webp
- alpha-quality: 80
- encoding: "auto"
- low-memory: true
- log-call-arguments: true
- metadata: "none"
- method: 6
- near-lossless: 60
- quality: 85
- use-nice: true
- command-line-options: ""
- try-common-system-paths: true
- try-supplied-binary-for-os: true

The following options have not been explicitly set, so using the following defaults:
- auto-filter: false
- default-quality: 85
- max-quality: 85
- preset: "none"
- size-in-percentage: null (not set)
- skip: false
- rel-path-to-precompiled-binaries: *****
- try-cwebp: true
- try-discovering-cwebp: true
------------

Encoding is set to auto - converting to both lossless and lossy and selecting the smallest file

Converting to lossy
Looking for cwebp binaries.
Discovering if a plain cwebp call works (to skip this step, disable the "try-cwebp" option)
- Executing: cwebp -version. Result: *Exec failed* (the cwebp binary was not found at path: cwebp)
Nope a plain cwebp call does not work
Discovering binaries using "which -a cwebp" command. (to skip this step, disable the "try-discovering-cwebp" option)
Found 0 binaries
Discovering binaries by peeking in common system paths (to skip this step, disable the "try-common-system-paths" option)
Found 1 binaries: 
- /usr/local/bin/cwebp
Discovering binaries which are distributed with the webp-convert library (to skip this step, disable the "try-supplied-binary-for-os" option)
Checking if we have a supplied precompiled binary for your OS (Darwin)... We do.
Found 1 binaries: 
- [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14
Detecting versions of the cwebp binaries found
- Executing: /usr/local/bin/cwebp -version. Result: version: *1.0.3*
- Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14 -version. Result: *Exec failed* (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14)
Binaries ordered by version number.
- /usr/local/bin/cwebp: (version: 1.0.3)
Trying the first of these. If that should fail (it should not), the next will be tried and so on.
Creating command line options for version: 1.0.3
Quality: 85. 
The near-lossless option ignored for lossy
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 85 -alpha_q '80' -m 6 -low_memory '[doc-root]/wp-content/uploads/2017/12/man-large.png' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/12/man-large.png.webp.lossy.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/12/man-large.png.webp.lossy.webp'
File:      [doc-root]/wp-content/uploads/2017/12/man-large.png
Dimension: 1024 x 498
Output:    70310 bytes Y-U-V-All-PSNR 41.35 45.99 43.94   42.24 dB
           (1.10 bpp)
block count:  intra4:       1181  (57.67%)
              intra16:       867  (42.33%)
              skipped:       154  (7.52%)
bytes used:  header:            532  (0.8%)
             mode-partition:   6175  (8.8%)
 Residuals bytes  |segment 1|segment 2|segment 3|segment 4|  total
  intra4-coeffs:  |   32071 |    3165 |    3257 |     661 |   39154  (55.7%)
 intra16-coeffs:  |    5212 |    4421 |    1408 |     504 |   11545  (16.4%)
  chroma coeffs:  |    9919 |    1672 |    1060 |     226 |   12877  (18.3%)
    macroblocks:  |      49%|      25%|      14%|      12%|    2048
      quantizer:  |      17 |      13 |       9 |       8 |
   filter level:  |       5 |       3 |       2 |       0 |
------------------+---------+---------+---------+---------+-----------------
 segments total:  |   47202 |    9258 |    5725 |    1391 |   63576  (90.4%)

Success
Reduction: 50% (went from 136 kb to 69 kb)

Converting to lossless
Looking for cwebp binaries.
Discovering if a plain cwebp call works (to skip this step, disable the "try-cwebp" option)
- Executing: cwebp -version. Result: *Exec failed* (the cwebp binary was not found at path: cwebp)
Nope a plain cwebp call does not work
Discovering binaries using "which -a cwebp" command. (to skip this step, disable the "try-discovering-cwebp" option)
Found 0 binaries
Discovering binaries by peeking in common system paths (to skip this step, disable the "try-common-system-paths" option)
Found 1 binaries: 
- /usr/local/bin/cwebp
Discovering binaries which are distributed with the webp-convert library (to skip this step, disable the "try-supplied-binary-for-os" option)
Checking if we have a supplied precompiled binary for your OS (Darwin)... We do.
Found 1 binaries: 
- [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14
Detecting versions of the cwebp binaries found
- Executing: /usr/local/bin/cwebp -version. Result: version: *1.0.3*
- Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14 -version. Result: *Exec failed* (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14)
Binaries ordered by version number.
- /usr/local/bin/cwebp: (version: 1.0.3)
Trying the first of these. If that should fail (it should not), the next will be tried and so on.
Creating command line options for version: 1.0.3
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 85 -alpha_q '80' -near_lossless 60 -m 6 -low_memory '[doc-root]/wp-content/uploads/2017/12/man-large.png' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/12/man-large.png.webp.lossless.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2017/12/man-large.png.webp.lossless.webp'
File:      [doc-root]/wp-content/uploads/2017/12/man-large.png
Dimension: 1024 x 498
Output:    120230 bytes (1.89 bpp)
Lossless-ARGB compressed size: 120230 bytes
  * Header size: 1385 bytes, image data size: 118819
  * Lossless features used: PALETTE
  * Precision Bits: histogram=4 transform=4 cache=2
  * Palette size:   256

Success
Reduction: 14% (went from 136 kb to 117 kb)

Picking lossy
cwebp succeeded :)

Converted image in 519 ms, reducing file size with 50% (went from 136 kb to 69 kb)
