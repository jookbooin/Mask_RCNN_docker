
## 1. scikit-build 설치 
![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/a2925018-da35-4532-b3c6-c57b3e861f4d)

```
pip install --upgrade pip
pip install scikit-build
pip install -r requirements.txt
```

</br>

## 2. numpy 1.18.5 →  1.16.4로 변경
```

ModuleNotFoundErrot: No module named 'numpy.testing.decorators' 발생
```
![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/12504ee9-3e4a-4bda-926a-09107ea2e7ec)

## 3. inspect_balloon_model.ipynb

* `BALLON_WEIGHTS_PATH` path 입력
  
  ![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/d39f717b-ae8b-4ebd-bb62-b936ad6306bc)

* `loadModel` weight_path 수정
  
  ![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/9395ea54-a2eb-44c9-8295-4dfd8c133e2a)

## 실행 결과 
`/root/Mask_RCNN` 의 `splash_20231122T040558.png` 
</br>

![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/bf3f41cd-d575-4759-a633-5d657f406bc5)

</br>

![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/33567888-6c6e-427d-b5f1-65c3988eb787)

</br>

![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/696a4f06-0514-44fe-87e9-1a3c6d0f63bc)


