# Attention Mechanisms Perspective: Exploring LLM Processing of Graph-Structured Data

![alt text](image.png)


[![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/pdf/2505.02130) 

```
@article{guan2025attention,
  title={Attention Mechanisms Perspective: Exploring LLM Processing of Graph-Structured Data},
  author={Guan, Zhong and Wu, Likang and Zhao, Hongke and He, Ming and Fan, Jianpin},
  journal={arXiv preprint arXiv:2505.02130},
  year={2025}
}


```




## 0. Python Environment Setup with Conda
```bash
conda create --name Exploration python=3.8
conda activate Exploration

pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
pip install torch==2.0.0+cu118 torchvision==0.15.1+cu118 torchaudio==2.0.1+cu118 -f https://download.pytorch.org/whl/torch_stable.html

pip install torch_geometric
pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu118.html

pip install ogb
pip install yacs
pip install transformers==4.31.0
pip install peft==0.4.0
pip install accelerate
pip install bitsandbytes==0.39.0
#pip install sentence_transformers    #sentence_transformers-3.0.1 tokenizers-0.19.1 transformers-4.44.2

pip install wheel

pip install torch_geometric

pip install SentencePiece
pip install protobuf
pip install bitsandbytes==0.39.0

pip install matplotlib==3.6.1  
pip install protobuf==3.19.6  
pip install accelerate==0.33.0  
pip install bitsandbytes==0.39.0
pip install dataset==1.6.2  
pip install datasets==2.21.0  

```

## 1. Download TAG Datasets

We provide both the raw text data and processed embeddings of our collected datasets on Google Drive. You can download them from:  
[Google Drive Link](https://drive.google.com/drive/folders/1gIguSsAhqqEeQor2pfxvzH-d4tzWADZF?usp=sharing)

## 2. Implementation Details

### Core Scripts
- **LLM_atten_initial.py**  
  Standard script for LLM processing of graph tasks
- **LLM_atten_pad.py**  
  Enhanced script with padding and shuffle operations
- **LLM_atten_atten.py**  
  Extended script with additional attention mechanisms

### Experimental Notebooks
- **LLM_cengji_A.ipynb**  
  Exploration code for Section A of the paper, including visualization
- **LLM_cengji_B.ipynb**  
  Exploration code for Section B of the paper, including visualization

---

**We welcome contributions!** Feel free to open an issue if you have any questions.

