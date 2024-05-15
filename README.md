
### Linux/Unix

1. Install [Anaconda](https://www.anaconda.com/), Python and `git`.

2. Creating the env and install the requirements.
  ```bash
  git clone https://github.com/OpenTalker/SadTalker.git

  cd SadTalker 

  conda create -n sadtalker python=3.8

  conda activate sadtalker

  pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 torchaudio==0.12.1 --extra-index-url https://download.pytorch.org/whl/cu113

  conda install ffmpeg

  pip install -r requirements.txt

  ### Coqui TTS is optional for gradio demo. 
  ### pip install TTS

  ```


### solve the errors : 

1. for fps related issue install fellowing version of the library :
```
pip install imageio==2.19.3
pip install imageio-ffmpeg==0.4.7 
```

or for more fellow this lnk 
https://github.com/OpenTalker/SadTalker/issues/276   \


3. if np.long related issue 
change the version of numpy to numpy==1.23.0 


4. for ValueError: input_path must be a valid path to video/image file
follow it I give instructions there : 

https://github.com/OpenTalker/SadTalker/issues/672



[![Watch the video](examples/source_image/ramveer.jpeg)](/examples/generated_video/ramveer.mp4)


