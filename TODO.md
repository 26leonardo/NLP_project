# TODO

## Statistics on the dataset

* [ ] Plot distributions, etc.

## General Cleanup

* [ ] Reduce redundancy in NLTK downloads and confirm only required resources are installed.
* [ ] Validate whether local `nltk_data` setup is necessary or can be simplified.

## Emoji Handling

* [ ] Optional: convert text-based emojis into textual placeholders instead of dropping them. We also would need not to remove them with regex.

## Regex and Pattern Design

* [ ] Clarify whether quotes should be filtered  in the dedicated pattern or uniformly under “non-alphanumeric.”
* [ ] Investigate replacing the full “non-alphanumeric” regex with a more selective filter to avoid over-cleaning.

## Train-Only Postprocessing

Apply additional cleaning steps only to the training set:

* [ ] Remove leftover noisy characters caused by naive removal rules.
* [ ] Compress repeated punctuation into single instances.
* [ ] Optionally detect and handle HTML tags or noisy patterns like `10%-`.

## Embeddings

* [ ] In the try-except case, try a more fitting strategy for missing embedding than random: interpolation.
