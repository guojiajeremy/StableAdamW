# StableAdamW
Unofficial implementation of StableAdamW, the hybrid of AdamW+AdaFactor.
[Stable and low-precision training for large-scale vision-language models](https://arxiv.org/pdf/2304.13013.pdf)

StableAdamW is proposed to stabilize Transformer training. 
This repository implement a little different version of StableAdamW.
Ours: $RMS_t=rms(g_t/denom)$, where denom is simply the denominator of AdamW with bias correction and epsilon.
