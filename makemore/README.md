# makemore

Character-level language models trained on ~32k names, following Karpathy's makemore series.

| Notebook | Model | Params | Train loss | Dev loss |
|---|---|---|---|---|
| [01_bigrams](01_bigrams.ipynb) | Bigram (counting) | 729 | 2.454 | - |
| [01_bigrams](01_bigrams.ipynb) | Bigram (neural net, 1 linear layer) | 729 | 2.490 | - |
| [02_mlp](02_mlp.ipynb) | MLP (Bengio et al. 2003), context 3, emb 10, hidden 200 | 11,897 | 2.128 | 2.170 |

The bigram models were trained on the full dataset, so they have no dev loss. From part 2 onward the data is split 80/10/10 into train/dev/test.

Data: `data/names.txt` from [karpathy/makemore](https://github.com/karpathy/makemore).
