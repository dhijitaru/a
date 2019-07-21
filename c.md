import cv2
import os
import numpy as np
import matplotlib.pyplot as plt
from skimage.io import imread, imsave
video = cv2.VideoCapture('WIN_20190722_02_46_40_Pro.mp4')
dir_name = "a"
if not os.path.exists(dir_name):
    os.mkdir(dir_name)
frame_count = int(video.get(7))
for i in range(frame_count):
    _, frame = video.read()
    cv2.imwrite(dir_name + "/" + str(i) + ".png", frame)
    
im0 = imread('a/0.png')
im1 = imread('a/1.png')
im2 = imread('a/2.png')
im3 = imread('a/3.png')
im4 = imread('a/4.png')
im5 = imread('a/5.png')
im6 = imread('a/6.png')
im7 = imread('a/7.png')
im8 = imread('a/8.png')
im9 = imread('a/9.png')
im10 = imread('a/10.png')
im11 = imread('a/11.png')
im12 = imread('a/12.png')
im13 = imread('a/13.png')
im14 = imread('a/14.png')
im15 = imread('a/15.png')
im16 = imread('a/16.png')
im17 = imread('a/17.png')
im18 = imread('a/18.png')
im19 = imread('a/19.png')
im20 = imread('a/20.png')
im21 = imread('a/21.png')
im22 = imread('a/22.png')
im23 = imread('a/23.png')
im24 = imread('a/24.png')
im25 = imread('a/25.png')
im26 = imread('a/26.png')
im27 = imread('a/27.png')
im28 = imread('a/28.png')
im29 = imread('a/29.png')
im30 = imread('a/30.png')


x = np.arange(0,31)
y=[im0.mean(),
   im1.mean(),
   im2.mean(),
   im3.mean(),
   im4.mean(),
   im5.mean(),
   im6.mean(),
   im7.mean(),
   im8.mean(),
   im9.mean(),
   im10.mean(),
   im11.mean(),
   im12.mean(),
   im13.mean(),
   im14.mean(),
   im15.mean(),
   im16.mean(),
   im17.mean(),
   im18.mean(),
   im19.mean(),
   im20.mean(),
   im21.mean(),
   im22.mean(),
   im23.mean(),
   im24.mean(),
   im25.mean(),
   im26.mean(),
   im27.mean(),
   im28.mean(),
   im29.mean(),
   im30.mean(),]

for z in range(30):
    print("in" + str(z) + "=" + str(y[z]))
    
    plt.plot(x,y)
    plt.show


説明
計算に必要なプログラムを取り入れる
自分のとった映像を取り入れる
映像から得られる画像の名前をaとする
フレームの数を数える
フレームの数まで映像を取り入れる
画像を30枚取り入れる
それぞれの画像の明るさの平均を計算する
得られた値をグラフにプロットする

使い方　コードをジュピターに載せる
実行の仕方　ctrl+Enter
ライブラリとバージョン
numpy                     1.16.4           py37h19fb1c0_0
matplotlib                3.1.0            py37hc8f65d3_0

参考
https://sorabatake.jp/5518/
サンプルコードの部分を参考にした

実行の様子
![digital.gif](digital.gif)
