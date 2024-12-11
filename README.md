# Ml/AI for Network Traffic Analysis FInal Project: Hidden Cam Inspector 

### Usage

```
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```


### Files:

- `ml_vs_statisticical_spike_detection.ipynb` contains all the code for loading the pre-processed data and performing analysis on the various flows, to recreate each trial 

- `datasets/camera_upload_traffic_updated.csv` contains all the upload traffic from each camera. Each trial is differentiated by a ID number, and the upload traffic is aggregated per second.

- `datasets/phone_noise_upload_traffic.csv` and `datasets/psmart_tv_upload_traffic.csv` contains the same data for the iphone traffic and smart TV traffic used in these experiments.

- The `results` folder consists of three .csv files containing the classification results from each of the three devices in every trial. 


### Results
| Camera Experiment                | True Pos | False Neg.|
|----------------------------------|--------|-------------|
| Standard Score - Original   |  0.69   | 0.31  |
| Standard Score - Smoothed  |     0.9 | 0.095  |
| ML - Original Trace              | 0.64  | 0.36
| ML - Smoothed Trace        | 0.62     | 0.3|
---

| Phone              | True Neg | False Pos |
|----------------------------------|--------|-------------|
| Standard Score - Original  |  0.82   | 0.18  |
| Standard Score - Smoothed  |     0.71 | 0.29  |
| ML - Original           | 0.82  | 0.18 |
| ML - Smoothed         | 0.82    | 018|
---

| TV             | True Neg | False Pos |
|----------------------------------|--------|-------------|
| Standard Score - Original  |  1.0  | 0.0 |
| Standard Score - Smoothed  |     0.76 | 0.24  |
| ML - Original           | 0.94 | 0.06
| ML - Smoothed         | 0.94    | 0.06|
___
