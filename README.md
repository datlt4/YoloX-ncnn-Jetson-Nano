# YoloX Jetson Nano
![output image]( https://qengineering.eu/images/test_parkX.webp )
## YoloX with the ncnn framework. <br/>
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>
Paper: https://arxiv.org/pdf/2107.08430.pdf<br/><br/>
Special made for a Jetson Nano, see [Q-engineering deep learning examples](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html)

------------

## Benchmark.
| Model  | size | objects | mAP | Jetson Nano | RPi 4 1950 MHz | Rock 5 |
| ------------- | :-----:  | :-----:  | :-----:  | :-------------:  | :-------------: | :-----: |
| [NanoDet](https://github.com/Qengineering/NanoDet-ncnn-Raspberry-Pi-4) | 320x320 | 80 | 20.6  |  26.2 FPS | 13.0 FPS | 36.0 FPS |
| [NanoDet Plus](https://github.com/Qengineering/NanoDetPlus-ncnn-Raspberry-Pi-4) | 416x416 | 80 | 30.4  |  18.5 FPS | 5.0 FPS | 24.9 FPS |
| [YoloFastestV2](https://github.com/Qengineering/YoloFastestV2-ncnn-Raspberry-Pi-4) | 352x352  | 80 | 24.1 |  38.4 FPS | 18.8 FPS | 65.4 FPS |
| [YoloV2](https://github.com/Qengineering/YoloV2-ncnn-Raspberry-Pi-4) | 416x416  | 20 | 19.2 |  10.1 FPS | 3.0 FPS | 20.0 FPS |
| [YoloV3](https://github.com/Qengineering/YoloV3-ncnn-Raspberry-Pi-4) | 352x352 tiny | 20 | 16.6 | 17.7 FPS | 4.4 FPS | 15.0 FPS |
| [YoloV4](https://github.com/Qengineering/YoloV4-ncnn-Raspberry-Pi-4) | 416x416 tiny | 80 | 21.7 | 16.1 FPS | 3.4 FPS | 22.4 FPS |
| [YoloV4](https://github.com/Qengineering/YoloV4-ncnn-Raspberry-Pi-4) | 608x608 full | 80 | 45.3 | 1.3 FPS | 0.2 FPS | 1.5 FPS |
| [YoloV5](https://github.com/Qengineering/YoloV5-ncnn-Raspberry-Pi-4) | 640x640 small| 80 | 22.5 | 5.0 FPS | 1.6 FPS | 12.5 FPS |
| [YoloV6](https://github.com/Qengineering/YoloV6-ncnn-Raspberry-Pi-4) | 640x640 nano | 80 | 35.0 | 10.5 FPS | 2.7 FPS | 20.8 FPS |
| [YoloV7](https://github.com/Qengineering/YoloV5-ncnn-Raspberry-Pi-4) | 640x640 tiny| 80 | 38.7 | 8.5 FPS | 2.1 FPS | 17.9 FPS |
| [YoloX](https://github.com/Qengineering/YoloX-ncnn-Raspberry-Pi-4) | 416x416 nano | 80 | 25.8 | 22.6 FPS | 7.0 FPS | 28.5 FPS |
| [YoloX](https://github.com/Qengineering/YoloX-ncnn-Raspberry-Pi-4) | 416x416 tiny | 80 | 32.8 | 11.35 FPS | 2.8 FPS | 18.1 FPS |
| [YoloX](https://github.com/Qengineering/YoloX-ncnn-Raspberry-Pi-4) | 640x640 small | 80 | 40.5 | 3.65 FPS | 0.9 FPS | 7.5 FPS |

------------

## Dependencies.
To run the application, you have to:
- The Tencent ncnn framework installed. [Install ncnn](https://qengineering.eu/install-ncnn-on-jetson-nano.html) <br/>
- OpenCV 64 bit installed. [Install OpenCV 4.5](https://qengineering.eu/install-opencv-4.5-on-raspberry-64-os.html) <br/>
- Code::Blocks installed. (```$ sudo apt-get install codeblocks```)

------------

## Installing the app.
To extract and run the network in Code::Blocks <br/>
$ mkdir *MyDir* <br/>
$ cd *MyDir* <br/>
$ wget https://github.com/Qengineering/YoloX-ncnn-Jetson-Nano/archive/refs/heads/main.zip <br/>
$ unzip -j master.zip <br/>
Remove master.zip, LICENSE and README.md as they are no longer needed. <br/> 
$ rm master.zip <br/>
$ rm LICENSE <br/>
$ rm README.md <br/> <br/>
Your *MyDir* folder must now look like this: <br/> 
parking.jpg <br/>
busstop.jpg <br/>
YoloX.cpb <br/>
yoloX.cpp <br/>
yoloxS.bin <br/>
yoloxS.param <br/>
yoloxT.bin <br/>
yoloxT.param <br/>
yoloxN.bin <br/>
yoloxN.param <br/>

------------

## Running the app.
To run the application load the project file YoloX.cbp in Code::Blocks.<br/> 
Next, follow the instructions at [Hands-On](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html#HandsOn).<br/><br/>
Many thanks to [nihui](https://github.com/nihui/) again!<br/><br/>
![output image]( https://qengineering.eu/images/test_busX.webp )

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 
