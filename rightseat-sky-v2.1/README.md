# RightSeat Sky v2.1 payload release

This directory is the immutable compressed payload backing the production RightSeat Sky v2.1 loader.

Production: https://rightseat-sky-pilot-mvp.vercel.app/

## Payload order

Read `payload-manifest.json`. Concatenate the listed UTF-8 text files, base64-decode the result, and gzip-decompress it to recover the complete self-contained HTML application.

Expected decompressed SHA-256:

`1594d97d1b94086a05740bddcb5e6810f1bb0d074a6bf89a02ffb77225d9ad40`

## Main feature

Quick Align automatically selects a bright, well-separated two-star reference pair, guides the pilot to each star, keeps the capture control on the main view, and reports `STAR ALIGNED · LIVE` only after the two-star residual gate passes.

The pilot still positively identifies and centers each real star. This is not a blind plate solver or approved navigation source.
