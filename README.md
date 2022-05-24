# DACON_Speech
![20220524_130710](https://user-images.githubusercontent.com/84311270/169978764-71a90a2e-7b8b-4649-a645-a18ad55cb606.png)
총 6개국(Africa, Australia, Canada, England, Hongkong, US)에서 녹음 된 음성을 바탕으로 accent를 분류하는 알고리즘 개발

## Dataset
6개국에서 녹음된 mp3 파일을 wav 파일로 변환하여 적재  
(모든 음성은 5초 이상의 길이를 갖고 있습니다.)  



1. train folder (14.5 GB)  
Africa folder (2500개의 wav 파일)  
Australia folder (1000개의 wav 파일)  
Canada folder (1000개의 wav 파일)  
England folder (10000개의 wav 파일)  
Hongkong folder (1020개의 wav 파일)  
US folder (10000개의 wav 파일)  


2. test folder (3.5 GB)  
임의로 추출된 6100개 wav 파일  

3. sample_submission.csv  
id : 1~6100까지 test 파일의 id  
국가별 음성의 accent 예측 확률을 기재  

4. train.csv


## Model
basic_CNN 모델과 2D_CNN 모델 등을 활용하여 다양한 시도를 하였으며 학습.

## Results
Public Score : 1.09514, Private Score : 1.09317로 최종 6등으로 수상.
![20220524_130755](https://user-images.githubusercontent.com/84311270/169979756-70204c36-1114-48f2-81e1-e24ed9759dad.png)

