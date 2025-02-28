# MODEL ZOO

## Kinetics 

| Dataset | architecture | depth | init | clips x crops | #frames x sampling rate | acc@1 | acc@5 | checkpoint | config |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |
| K400 | TAda2D | R50 | IN-1K | 10 x 3 | 8 x 8 | 76.3 | 92.4 | [[google drive](https://drive.google.com/file/d/1-_Yek3lFYpgahU2Q2ITON4rgqm5Voj2E/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1CzJ82frDeH8P4L55aZdZ-Q)(code:jp7d)] |  configs/projects/tada/k400/tada2d_8x8.yaml |
| K400 | TAda2D | R50 | IN-1K | 10 x 3 | 16 x 5 | 76.9 | 92.7 | [[google drive](https://drive.google.com/file/d/1Phj2mSna27Gv46tJzjw4a51_qum1HW6x/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1GQZmB_ZKwq1NjmVooICa2w)(code:buww)] | configs/projects/tada/k400/tada2d_16x5.yaml |
| K400 | ViViT Fact. Enc. | B16x2 | IN-21K | 4 x 3 | 32 x 2 | 79.4 | 94.0 | [[google drive](https://drive.google.com/file/d/1xD4uij9DmZojnl1xuWBa-gwm5hUZxDc7/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1iVjKjEMm-6ymUd15ZNqvXw)(code:1t51)] | configs/projects/competition/k400/vivit_fac_enc_b16x2.yaml |

## Something-Something
| Dataset | architecture | depth | init | clips x crops | #frames | acc@1 | acc@5 | checkpoint | config |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |
| SSV2 | TAda2D | R50 | IN-1K | 2 x 3 | 8 | 63.8 | 87.7 | [[google drive](https://drive.google.com/file/d/1_OwuPjnVXNoOjkQ2q0NcmSWxCZJGgFTf/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1ITcHcYL6RCN2C7TP_v6cRg)(code:su94)] | configs/projects/tada/ssv2/tada2d_8f.yaml | 
| SSV2 | TAda2D | R50 | IN-1K | 2 x 3 | 16 | 65.2 | 89.1 | [[google drive](https://drive.google.com/file/d/1mwINu9ZFUMk1bHt47Xq9CDNnb07PCkG7/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1hXKpTSSpoVDBWpHWhKgjTg)(code:k03n)] | configs/projects/tada/ssv2/tada2d_16f.yaml | 

## Epic-Kitchens Action Recognition

| architecture | init | resolution | clips x crops | #frames x sampling rate | action acc@1 | verb acc@1 | noun acc@1 | checkpoint | config |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | 
| ViViT Fact. Enc.-B16x2 | K700 | 320 | 4 x 3 | 32 x 2 | 46.3 | 67.4 | 58.9 | [[google drive](https://drive.google.com/file/d/1ELvwZYeqdsPmDcX1v7_RbFqbQnvHt9sB/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1zOtIAY6neFshmkPR9SuX8g)(code:rinh)] | configs/projects/competition/ek100/vivit_fac_enc.yaml |
| ir-CSN-R152 | K700 | 224 | 10 x 3 | 32 x 2 | 44.5 | 68.4 | 55.9 | [[google drive](https://drive.google.com/file/d/1YEIhijzN2aFXyfDL34WB6Q9strYP7WaU/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1swVIBJInQ75dUZKV-OJwlg)(code:s0uj)] | configs/projects/competition/ek100/csn.yaml | 

## Epic-Kitchens Temporal Action Localization

| feature | classification | type | IoU@0.1 | IoU@0.2 | IoU@0.3 | IoU@0.4 | IoU@0.5 | Avg | checkpoint | config |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | 
| ViViT | ViViT | Verb | 22.90 | 21.93 | 20.74 | 19.08 | 16.00 | 20.13 | [[google drive](https://drive.google.com/file/d/1O0-kPlPrPfrOiFyFcNbCDbnTfsflFc5z/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1sBu5puPU8mSqklYzsAzZWg)(code:3sud)]| configs/projects/epic-kitchen-tal/bmn-epic/vivit-os-local.yaml |
| ViViT | ViViT | Noun | 28.95 | 27.38 | 25.52 | 22.67 | 18.95 | 24.69 | [[google drive](https://drive.google.com/file/d/1O0-kPlPrPfrOiFyFcNbCDbnTfsflFc5z/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1sBu5puPU8mSqklYzsAzZWg)(code:3sud)]| configs/projects/epic-kitchen-tal/bmn-epic/vivit-os-local.yaml |
| ViViT | ViViT | Action | 20.82 | 19.93 | 18.67 | 17.02 | 15.06 | 18.30 | [[google drive](https://drive.google.com/file/d/1O0-kPlPrPfrOiFyFcNbCDbnTfsflFc5z/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1sBu5puPU8mSqklYzsAzZWg)(code:3sud)]| configs/projects/epic-kitchen-tal/bmn-epic/vivit-os-local.yaml |
| TAda2D | TAda2D | Verb | 19.70 | 18.49 | 17.41 | 15.50 | 12.78 | 16.78 | [[google drive](https://drive.google.com/file/d/13VhZhUN5p3j7Y0X7ZMQb83dncEx_DBVI/view?usp=sharing)][[baidu](https://pan.baidu.com/s/11Mzrb8qBTF9j-WJaxhf5yw)(code:d01j)]| - | 
| TAda2D | TAda2D | Noun | 20.54 | 19.32 | 17.94 | 15.77 | 13.39 | 17.39 | [[google drive](https://drive.google.com/file/d/13VhZhUN5p3j7Y0X7ZMQb83dncEx_DBVI/view?usp=sharing)][[baidu](https://pan.baidu.com/s/11Mzrb8qBTF9j-WJaxhf5yw)(code:d01j)]| - | 
| TAda2D | TAda2D | Action | 15.15 | 14.32 | 13.59 | 12.18 | 10.65 | 13.18 | [[google drive](https://drive.google.com/file/d/13VhZhUN5p3j7Y0X7ZMQb83dncEx_DBVI/view?usp=sharing)][[baidu](https://pan.baidu.com/s/11Mzrb8qBTF9j-WJaxhf5yw)(code:d01j)]| - | 

## MoSI
Note: for the following models, decord 0.4.1 are used rather than the default 0.6.0 for the codebase.

### Pre-train (without finetuning)
| dataset | backbone | checkpoint | config |
| ------- | -------- | ---------- | ------ |
| HMDB51  | R-2D3D-18 | [[google drive](https://drive.google.com/file/d/18wnkUdekhaHGGghjtd77857RA0Ame4oo/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1X3P4jQyuw2AWP-uRgw3YAA)(code:ahqg)]| configs/projects/mosi/pt-hmdb/r2d3ds.yaml |
| HMDB51  | R(2+1)D-10 | [[google drive](https://drive.google.com/file/d/1dbBF0cokI_nCnKaImvXurtYuRQt1jkit/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1K8GyPIkG9KbDnQqi65ObFQ)(code:1ktb)]| configs/projects/mosi/pt-hmdb/r2p1d.yaml |
| UCF101  | R-2D3D-18 | [[google drive](https://drive.google.com/file/d/1-UVwSM7fsk5zDhc24Iy_WODPo9BafNQw/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1S6fiqyf5lNpRfbouV6Nugw)(code:61uw)]|configs/projects/mosi/pt-ucf/r2d3ds.yaml |
| UCF101  | R(2+1)D-10 | [[google drive](https://drive.google.com/file/d/1DxuNtGSxeuTAygR-eXlAT6JOM-nXZ6dT/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1TEzpmvmAsN81VqqGu81hhA)(code:drq2)]| configs/projects/mosi/pt-ucf/r2p1d.yaml | 

### Finetuned
| dataset | backbone | acc@1 | acc@5 | checkpoint | config |
| ------- | -------- | ----- | ----- | ---------- | ------ |
| HMDB51  | R-2D3D-18 | 46.93 | 74.71 | [[google drive](https://drive.google.com/file/d/1A77b3uwxWwlCj0rm7uQcn6m0-uVCUeWQ/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1LfO1fvQ2DD1uoRfS2MH6dA)(code:2puu)]| configs/projects/mosi/ft-hmdb/r2d3ds.yaml | 
| HMDB51  | R(2+1)D-10 | 51.83 | 78.63 | [[google drive](https://drive.google.com/file/d/1OOkooh6_GNsyF_1EolgboN9MFE0O2N2n/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1IhkUv7q7w0JW1ZyuBYgrBA)(code:hgnc)]| configs/projects/mosi/ft-hmdb/r2p1d.yaml |
| UCF101  | R-2D3D-18 | 71.75 | 89.14 | [[google drive](https://drive.google.com/file/d/1cwM4Zi0VUGpaiw3mCQcfe1A1aluIppaq/view?usp=sharing)][[baidu](https://pan.baidu.com/s/182JbBWwFFiM6dzmCloeB3A)(code:ndt6)]| configs/projects/mosi/ft-ucf/r2d3ds.yaml | 
| UCF101  | R(2+1)D-10 | 82.79 | 95.78 | [[google drive](https://drive.google.com/file/d/1cz_SMKFqvNyh_uEH8QOyomBf0MhOGN7Y/view?usp=sharing)][[baidu](https://pan.baidu.com/s/1B4h4XwZ_bQKcObP8E-6YAQ)(code:ecsf)]| configs/projects/mosi/ft-ucf/r2p1d.yaml |