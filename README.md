# Vowel recognition system based on mouth gesture and sound

Group Project for the Sound Communication class of the Sound and Music Coputing Master at the Music Technology Group, Universitat Pompeu Fabra, Barcelona.

## Description

This project is a *proof-of-concept* for a vowel recognition system based on mouth gesture and sound. 
The system is based on the following steps:

```tree
audio-in (Audio input captured with Python)                     FaceOSC (Face tracking)
    |                                                                       |
audio feature extraction (Python?)                            mouth gesture extraction (Python)
    |                                                                       |
   OSC                                                                     OSC
    |                                                                       |                                           
    --------------------------->    Wekinator       <------------------------
                                (Vowels recognition)
                                        |
                                        |
                                       OSC
                                        |
                                    Max / MSP
                        (visual feedback and audio examples)
```

## Goals (work in progress)

The purpose of this project is to create a working infra-structure that could support language teaching applications.

7 possible vowels sounds are considered: /a/, /e/, /i/, /o/, /u/, /y/, /ø/.

## Run this code

1. install Wekinator

1. install FaceOSC (optional)

1. run from terminal:

    ```bash
    pip3 install -r requirements.txt

    python3 audio_osc_wekinator.py
    ```

1. open Wekinator > File > Open > [project file](./WekinatorProject/WekinatorProject.wekproj)

1. run the pre-trained model