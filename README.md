# [MinRNNs for Lagrangian-Based Simulations of Transient Flow Problems](http://dx.doi.org/10.1007/978-3-031-97554-7_17)

This is the official repository for the paper [*MinRNNs for Lagrangian-Based Simulations of Transient Flow Problems*](http://dx.doi.org/10.1007/978-3-031-97554-7_17).  
This repository contains the code for the surrogate model of 2D Lagrangian fluid and multimaterial simulations.

The repository also includes the [appendix of the paper](https://github.com/dodydharma/minRNNsFlow/blob/main/docs/appendix.pdf) in the `docs` directory.

---

![Qualitative Results](https://github.com/dodydharma/minRNNsFlow/blob/main/docs/gif/qualitative-results.gif)

*Qualitative results: minLSTM/minGRU train 350–400% faster than LSTM/GRU, matching or surpassing their accuracy.*

---

![Snapshots from groundtruth data for multi-material multi-phase simulation.  
Top-left: homogeneous liquid; top-middle: snow; top-right: rope and jelly ball;  
bottom-left: liquid and snow; bottom-middle: rope and snow; bottom-right: rope and liquid.](https://media.springernature.com/full/springer-static/image/chp%3A10.1007%2F978-3-031-97554-7_17/MediaObjects/667304_1_En_17_Fig1_HTML.png?as=webp)

*Snapshots from groundtruth data for multi-material multi-phase simulation. Top-left: homogeneous liquid; top-middle: snow; top-right: rope and jelly ball; bottom-left: liquid and snow; bottom-middle: rope and snow; bottom-right: rope and liquid.*

---

## Abstract

Motivated by the need for faster yet accurate surrogate modeling of continuum simulations, we investigate whether the recently proposed minimal recurrent networks (minLSTM and minGRU [1] (also available at https://github.com/BorealisAI/minRNNs)) can benefit particle-based fluid and soft-solid simulations. To our knowledge, this is the first work applying these minimal RNNs to Lagrangian data from 2D continuum simulation, including single-phase fluids and multi-material interactions. We embed minLSTM and minGRU in an MLP-based encoder–decoder and compare them against (i) a classical LSTM, and (ii) an MLP baseline with no recurrent core. Where prior studies of minRNNs focused on simpler time-series tasks, our results show that minLSTM and minGRU remain highly effective in these physics-driven settings: they train approximately 350–400% faster than the standard LSTM or GRU, while matching—and often surpassing—their accuracy. Thus, for particle-based continuum simulations, minimal recurrent architectures offer a superior trade-off between computational overhead and predictive performance, thereby advancing real-time or high-fidelity simulation workflows in engineering and visual effects. We conclude that minimal RNNs are well-suited for surrogate modeling of fluid and soft-solid dynamics.
