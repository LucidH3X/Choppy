<img width="1200" height="630" alt="image" src="https://github.com/user-attachments/assets/f2092058-fb30-44f7-ae03-b22c9fc76385" />

Split big CSV files into pieces that fit under an upload limit (default 29.5 MB), then download them all as one zip.

- Every piece keeps the header row
- Rows are never cut in half, even when quoted fields contain commas or line breaks
- Bytes are copied exactly, so line endings, encoding and BOM are kept as they were
- Drop single files or a whole folder
- **It runs 100% in the browser. Nothing is uploaded and there's no server.**

## Use it

Open the page, set the max size, drop your CSVs in, and click **Chop & download zip**.


## Limits

- The finished zip has to be under 4 GB.
- Very large batches are held in browser memory while the zip is built. Chrome and Firefox handle hundreds of MB fine.
- It needs a modern browser: Chrome/Edge 103+, Firefox 113+ or Safari 16.4+. Older browsers still work but the zip won't be compressed.

