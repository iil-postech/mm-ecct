# Multiple-Masks Error Correction Code Transformer for Short Block Codes

This repository provides the official implementation of the IEEE Journal on Selected Areas in Communications "Multiple-Masks Error Correction Code Transformer for Short Block Codes"

# [Paper](https://doi.org/10.1109/JSAC.2025.3559154)
<p align="center"><img src="https://github.com/user-attachments/assets/7311e9e4-ff7e-4c3d-9ffd-de359e825214" width="400"/>

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
@article{Park2024multiple,
  title = {Multiple-Masks Error Correction Code Transformer for Short Block Codes},
  author = {Park, Seong-Joon and Kwak, Hee-Youl and Kim, Sanghyo and Kim, Sunghwan and Kim, Yongjune and No, Jong-Seon},
  journal = {IEEE Journal on Selected Areas in Communications (JSAC)},
  volume = 43,
  number = 7,
  page = {2518--2529},
  month = jul,
  year={2025}
}
```

# License

Codes are available only for non-commercial research purposes.

# Acknowledgement

This repository is based on [***ECCT***](https://github.com/yoniLc/ECCT).
