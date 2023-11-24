
# 📌docker image
docs에서 제공하는 image 사용

![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/70baff49-d462-435b-875a-eaf27ef22bc9)


# 📌scikit-build 설치 
![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/a2925018-da35-4532-b3c6-c57b3e861f4d)

```
pip install --upgrade pip
pip install scikit-build
pip install -r requirements.txt
```

</br>

# 📌numpy 1.18.5 →  1.16.4로 변경
```

ModuleNotFoundErrot: No module named 'numpy.testing.decorators' 발생
```
![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/12504ee9-3e4a-4bda-926a-09107ea2e7ec)

# 📌data set 
![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/34e5aacf-fcbe-4ba9-b71e-0594102ee546)


* `mask_rcnn_balloon.h5` 는 `Mask_RCNN root 폴더 밑`에 위치
  
  ![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/1ca055e4-1a47-4a53-998a-df89781f32de)

* ballon 이미지 `Mask_Rcnn\datasets` 내부에 위치
  
  ![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/81c0eafd-d170-4ab9-a611-6cd1e25df3d2)


# 📌 학습 시도...?
링크에서 제공된 내용을 이용해서 학습해보려고 다음 을 이용했음 

![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/f39b602a-b3ec-41a4-a41b-63394380df79)

## 😢결과 
```
python3 samples/balloon/balloon.py train --dataset=/root/Mask_RCNN/datasets/balloon --weights=coco
```

![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/7b7940e7-915a-4a55-b0f2-fdfe572a59a7)

![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/d72a5e0d-dae2-4a79-972a-9e22c271c2e9)




# 📌 `mask_rcnn_balloon.h5` 실행 결과 
`/root/Mask_RCNN` 의 `splash_20231122T040558.png` 
</br>
```
root@c0030142e856:~/Mask_RCNN# python3  samples/balloon/balloon.py splash --weights=/path/to/mask_rcnn/mask_rcnn_balloon.h5 --image=datasets/balloon/val/3800636873_ace2c2795f_b.jpg
```
![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/bf3f41cd-d575-4759-a633-5d657f406bc5)

# 📌실행 결과


## 📘`inspect_balloon_model.ipynb ` 수정사항

* `BALLON_WEIGHTS_PATH` path 입력
  
  ![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/d39f717b-ae8b-4ebd-bb62-b936ad6306bc)

* `loadModel` weight_path 수정
  
  ![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/9395ea54-a2eb-44c9-8295-4dfd8c133e2a)


</br>

![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/33567888-6c6e-427d-b5f1-65c3988eb787)

</br>

![image](https://github.com/jookbooin/Mask_RCNN_docker/assets/94632156/696a4f06-0514-44fe-87e9-1a3c6d0f63bc)


