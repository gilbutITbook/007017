# <머신 러닝을 다루는 기술 with 파이썬, 사이킷런>(길벗, 2020) 도서의 예제 파일입니다.

## 환경 설정 방법

## 전체 실습 환경 설정
1. Anaconda를 설치합니다. <br/>
https://www.anaconda.com/distribution/#download-section

2. Anaconda Prompt(Command Line Interface 도구)를 열어 실습 파일이 있는 폴더(예: mlwpy_kor)로 이동합니다. <br/>
$ cd mlwpy_kor

3. book_base라는 이름으로 가상 환경을 설정하고 파이썬 3.7을 쓰도록 설정합니다. <br/>
$ conda create -n book_base python=3.7

4. 생성한 가상 환경 book_base로 들어갑니다.<br/>
$ conda activate book_base

5. 다음과 같이 필요한 라이브러리를 설치합니다. 한 줄씩 실행해주세요. 실행하면 설치하겠느냐는 y/n이 나옵니다. y를 입력하고 엔터키를 누르세요.<br/>
$ conda install matplotlib=3.1.0 <br/>
$ conda install pandas=0.25.0 <br/>
$ conda install numpy==1.16.4 <br/>
$ conda install patsy=0.5.1 <br/>
$ conda install scikit-learn=0.21.2 <br/>
$ conda install scipy=1.3.1 <br/>
$ conda install seaborn=0.9.0 <br/>
$ conda install statsmodels=0.10.1 <br/>
$ conda install tensorflow=1.14.0 <br/>
$ conda install opencv=3.4.2 <br/>
$ conda install scikit-image=0.16.2 <br/>
$ conda install pydotplus=2.0.2 <br/>
$ conda install graphviz <br/>
$ conda install jupyter <br/>
$ conda install memory_profiler <br/>
$ conda install py-xgboost=0.90 <br/>

6. 앞에서 만든 가상 환경을 ipython kernel로 등록합니다. <br/>
$ python -m ipykernel install --user --name book_base 

7. 주피터 노트북을 실행하면 인터넷 브라우저에서 노트북을 이용할 수 있습니다.  <br/>
$ jupyter notebook

## 15장 실습 환경 설정
15장에서는 pymc3와 keras를 추가로 설치한 후 실습을 진행해야 합니다. 이 책의 저자는 실습 오류를 방지하기 위해 15장부터는 별도의 가상 환경을 추가로 만들어 실습하길 권장합니다. 앞의 실습에 이어서 필요한 두 라이브러리만 추가로 설치한 후 실습해도 되고, 별도의 가상 환경을 추가로 만들어 실습해도 됩니다.

### 앞의 실습에 이어 실습
1. 다음처럼 두 라이브러리를 추가로 설치합니다.  <br/>
$ conda install pymc3   <br/>
$ conda install keras=2.3.1   <br/>

2. 15장의 주피터 노트북 파일을 실행하면 커널 경고 화면이 뜹니다. 'book_base'로 선택한 후 'Set Kernel'을 클릭합니다.  

3. 이어서 실습을 진행합니다.

### 별도의 가상 환경을 추가해 실습 
1~3단계는 '전체 실습 환경 설정'과 동일하게 진행합니다. 

4. book_base_pymc3라는 이름으로 가상 환경을 설정하고 파이썬 3.7을 쓰도록 설정합니다.  <br/>
$ conda create -n book_base_pymc3 python=3.7

5. 생성한 가상 환경 book_base_pymc3로 들어갑니다.  <br/>
$ conda activate book_base_pymc3

6. '전체 실습 환경 설정'의 6단계에서 소개한 모든 라이브러리를 설치합니다. 마지막으로 pymc3와 keras를 추가로 설치합니다.  <br/>
$ conda install pymc3     <br/>
$ conda install keras=2.3.1

7. 앞에서 만든 가상 환경을 ipython kernel로 등록합니다.  <br/>
$ python -m ipykernel install --user --name book_base_pymc3

8. 주피터 노트북을 실행하면 인터넷 브라우저에서 노트북을 이용할 수 있습니다.  <br/>
$ jupyter notebook

- 실습에 필요한 101_ObjectCategories 파일은 [여기](https://github.com/gilbutITbook/007017/releases/download/0.1/101_ObjectCategories.tar.gz)를 클릭해도 내려받을 수 있습니다.
- 자세한 실습 환경 설정 방법은 책의 부록 B를 참고하세요.