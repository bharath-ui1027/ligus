# Third-party notices

Ligus is an independent product by Bharath Sai Kondaveeti. It is not
affiliated with, endorsed by, or sponsored by Convai Innovations,
Microsoft, Google, OpenAI, or Anthropic.

## Laya (Apache License 2.0)

The relevance judges in Ligus are built on **Laya**, an open-source
decision engine by Convai Innovations:

- Source: https://github.com/NandhaKishorM/laya
- Copyright: Convai Innovations
- License: Apache License 2.0 — full text in `APACHE-2.0.txt`

The bundled `checkpoint/` model is a fine-tune created by the Ligus
author using Laya, and is distributed under this product's LICENSE.
The base Stage-2 model (`convaiinnovations/laya`) is bundled in
`base_model/` under the Apache License 2.0; if that folder is removed,
Ligus downloads it from Hugging Face on first use instead.

## all-MiniLM-L6-v2 (Apache License 2.0)

The bundled `models/` embedding model is
`sentence-transformers/all-MiniLM-L6-v2` exported to ONNX, used for the
local document index.

- Source: https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2
- License: Apache License 2.0 — full text in `APACHE-2.0.txt`

## Python libraries

Python dependencies (PyTorch, Transformers, Flask, and others) are
downloaded from PyPI during installation and are **not** bundled with
Ligus. Each is governed by its own license, shown on its PyPI page and
in the installed `venv` folder.
