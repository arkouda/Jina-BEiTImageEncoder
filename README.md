# BEiTImageEncoder

BEiTImageEncoder embeds images into 768-dim vectors using Bert Pre-trained ViT by Microsoft

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

- To override `__init__` args & kwargs, use `.add(..., uses_with: {'key': 'value'})`
- To override class metas, use `.add(..., uses_metas: {'key': 'value})`
