# RHGN
Source code for CIKM 2021 paper for [Relation-aware Heterogeneous Graph for User Profiling](https://arxiv.org/abs/2110.07181)
# Dependencies
torch==1.6.0 <br>
torchvision==0.7.0 <br>
dgl==0.7.1 <br>
scikit-learn==0.23.2 <br>
numpy==1.19.1 <br>
scipy ==1.5.2 <br>
pandas==1.1.2 <br>
# Dataset

Processed data download link: [Dataset](https://drive.google.com/drive/folders/1K0tRyHOOB63PnXtFtwLU5eM2NbRTiKXG?usp=sharing)<br>
Raw data and more details in [JD-Dataset](https://github.com/guyulongcs/IJCAI2019_HGAT) and [Alibaba-dataset](https://tianchi.aliyun.com/dataset/dataDetail?dataId=56)

# Usage
### For processed data:
```
python tb_tmain.py --data_dir ../taobao_data/ --model RHGN --label gender --graph G_ori --gpu 3  # Alibaba-Dataset

python jd_tmain.py --data_dir ../data/ --model RHGN --graph G_ori  --label age --gpu 2  # JD-Dataset

```
### How to process data
```
python process.py --data_dir ../taobao_data/    #Alibaba-Dataset

python process.py --data_dir ../data/    #JD-Dataset
```
More command can refer  run.sh and baseline.sh
# Contact
qilong.yan@cripac.ia.ac.cn
