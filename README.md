
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

1. for fps related issue fellow this link :  
https://github.com/OpenTalker/SadTalker/issues/276   \


2. if np.long related issue 
change the version of numpy to numpy==1.23.0 


3. for ValueError: input_path must be a valid path to video/image file
follow it I give instructions there : 

https://github.com/OpenTalker/SadTalker/issues/672





