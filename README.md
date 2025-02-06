# Multiple-Masks Error Correction Code Transformer for Short Block Codes

This repository is the official implementation of the IEEE Journal on Selected Areas in Communications "Multiple-Masks Error Correction Code Transformer for Short Block Codes"

# [Paper](https://arxiv.org/abs/2308.08128)
<p align="center"><img src="https://github.com/user-attachments/assets/c195180e-580e-4ffc-85d2-75b43dd53ac9" width="400"/>

# Experimental Results
<p align="center"><img src="https://github.com/user-attachments/assets/011f01df-7d15-4d44-a277-184a416a02c1" width="600"/>
  
BER performances of non-systematic mask (NSM) ECCT, systematic mask (SM) ECCT, multiple-masks (MM) ECCT with $$m=2$$ and MM ECCT with complementary double-masks (CDM). (a) (31,16) BCH code and (b) (63,30) BCH code for $$N=6$$ and $$d=128$$.

# Installation
* Pytorch

# Running the code

Codes for training DM ECCT on GPU 0, 3 decoder layers, dimension 128 on BCH codes (31,11)

```python
python Main.py --ecct_type=DM --gpu=0 --N_dec=3 --d_model=128 --code_type=BCH --code_n=31--code_k=11
```

# Code arguments
```
--ecct_type                ECCT type, 'SM' (systematic mask) or 'DM' (MM ECCT with double-masks)
--epochs                   number of epoch
--batch_size               batch size
--code_type                code type, 'BCH' or 'POLAR'
--code_k                   codeword dimension k
--code_n                   codeword length n
--N_dec                    number of decoder layers N
--d_model                  embedding vector dimension d
```

# Citation

```
@article{Park2024Multiple,
  title={Multiple-Masks Error Correction Code Transformer for Short Block Codes},
  author={Park, Seong-Joon and Kwak, Hee-Youl and Kim, Sanghyo and Kim, Sunghwan and Kim, Yongjune and No, Jong-Seon},
  journal={arXiv preprint arXiv:2405.01033},
  year={2025}
}
```

# License

Codes are available only for non-commercial research purposes.

# Acknowledgement

This repository is based on [***ECCT***](https://github.com/yoniLc/ECCT).
