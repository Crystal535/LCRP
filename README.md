## LCRP  
### Demo Video
<p float="left">
  <img src="demo/video_1.gif" width="45%" />
  <img src="demo/video_2.gif" width="45%" />
</p>

### More ablation studies
- Ref-DAVIS17

<div style="display:flex; gap:20px;">

<div>

| $N$   | $K$   | $J \& F$   |
|-------|-------|-------|
| 5 | 5 | 75.1 |
| 7 | 3 | 75.0 |
| 5 | 3 | 75.9 |
| **10**| **3** | **76.7** |
| 10| 5 | 76.3 |

</div>

<div>

| $H$   | $ \delta $   | $J \& F$   |
|-------|-------|-------|
| 1 | 0.1% | 76.5 |
| 2 | 0.3% | 76.6 |
| **3** | **0.3%** | **76.7** |
| 2| 0.2%| 76.5|
| 3| 0.2%| 76.5|

</div>

</div>

- MeViS

<div style="display:flex; gap:20px;">

<div>

| $N$   | $K$   | $J \& F$   |
|-------|-------|-------|
| 5 | 5 | 47.8 |
| 10 | 10 | 48.8 |
| 10 | 3 | 48.7 |
| **10** | **5** | **49.1** |
| 20 | 5 | 48.8 |

</div>

<div>

| $H$   | $ \delta $   | $J \& F$   |
|-------|-------|-------|
| 3 | 0.1% | 48.9 |
| **3** | **0.3%** | **49.1** |
| 2 | 0.3% | 48.9 |
| 2 | 0.2% | 48.7 |

</div>

</div>

### Model Complexity and Resource Usage on Ref-Youtube-VOS
| Method | Learnable params | Training GPU Memory Usage |Inference GPU Memory Usage |
|:--------:|:-----------------:|:--------------:|:--------------:|
| SOC | ~110.0 M | ~26 G | ~19 G |
| ReferDINO | ~15.3 M | ~21 G | ~12 G |
| Ours | 0 | 0 | ~15 G |
> **Note:** Both SOC and ReferDINO are trained and inferred on an **A100-40G GPU** with `batch_size=1`.  
> Our model is inferred on a single **RTX 4090-24G GPU** with `batch_size=1`.

### Segmentation Results 
- Binary Segmentation Results of Fig. 4.
![](demo/Figure%204.png)

### The code will be released soon






