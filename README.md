# REALITY
  
  
## Function  
 
### toImages(): 
#### 동영상을 이미지로 변환해주는 함수.

Args:
    - img_path: 변환할 이미지를 저장할 경로.
    - input_video_file: 이미지로 변환할 비디오 경로.

Returns:
  
  
### runDetector(): 
#### 이미지에서 객체를 탐지하는 함수(Faster-RCNN 적용).

Args:
    - detector: 객체 탐지 모듈
    - path: 모듈을 적용시킬 이미지 파일의 경로

Returns:
    - df: 프레임별 탐지된 객체들의 위치 정보가 담긴 DataFrame  
    
### objectIndexing(): 
#### 같은 Class에 속하는 객체들을 구분하여 id값을 지정해주는 함수

Args:
    - output_df: run_detector()의 return 값으로 전달된 DataFrame

Returns:
    - 객체들의 id 값이 담긴 list
    
    
## output file (reality_data.txt)  
id : 같은 객체끼리 같은 값을 가지는 객체의 고유값  
x : 객체 위치의 x좌표  
y : 객체 위치의 y좌표  
