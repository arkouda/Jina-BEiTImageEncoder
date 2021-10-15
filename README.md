# BEiTImageEncoder

``BEiTImageEncoder`` is an image encoder that wraps the image embedding functionality using the [BEiT]((https://arxiv.org/pdf/2106.08254.pdf)) models by Microsoft. The models have been implemented in HuggingFace transformers [here]((https://huggingface.co/transformers/model_doc/beit.html))

Supported Models:

- microsoft/beit-base-patch16-224-pt22k-ft22k
- microsoft/beit-base-patch16-224
- microsoft/beit-base-patch16-224-pt22k
- microsoft/beit-base-patch16-384
- microsoft/beit-large-patch16-224-pt22k-ft22k
- microsoft/beit-large-patch16-512
- microsoft/beit-large-patch16-224-pt22k
- microsoft/beit-large-patch16-224
- microsoft/beit-large-patch16-384

## Usage

#### via Docker image (recommended)

```python
from jina import Flow
	
f = Flow().add(uses='jinahub+docker://BEiTImageEncoder')
```

#### via source code

```python
from jina import Flow
	
f = Flow().add(uses='jinahub://BEiTImageEncoder')
```