# AI-Cover-Generator WebUI

AI-Cover-Generator is a Colab-based tool that allows users to generate custom album covers using AI models. The tool is designed to be easy to use, with a simple "Run all" option in Google Colab to start generating AI-based artwork.

## Features
- **AI-powered album cover generation**: Generate unique and creative cover art for albums or other creative projects.
- **Gradio WebUI**: Easy-to-use interface powered by Gradio for interacting with the model.
- **Voice Separation and Hubert Base Models**: The tool includes pre-trained models for voice separation and Hubert Base Model integration.

## How to Use

### Try it on Colab
[![Open in Colab](https://camo.githubusercontent.com/96889048f8a9014fdeba2a891f97150c6aac6e723f5190236b10215a97ed41f3/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/github/SociallyIneptWeeb/AICoverGen/blob/main/AICoverGen_colab.ipynb)

### Step 1: Clone the Repository
Simply copy the repository and run the following code to clone it in your environment:

```python
from IPython.display import clear_output, Javascript
import codecs
import threading
import time

cloneing=codecs.decode('uggcf://tvguho.pbz/FbpvnyylVarcgJrro/NVPbireTra.tvg','rot_13')
!git clone $cloneing HRVC
def update_timer_and_print():
    global timer
    while True:
        hours, remainder = divmod(timer, 3600)
        minutes, seconds = divmod(remainder, 60)
        timer_str = f'{hours:02}:{minutes:02}:{seconds:02}'
        print(f'\rTimer: {timer_str}', end='', flush=True)
        time.sleep(1)
        timer += 1

timer = 0
threading.Thread(target=update_timer_and_print, daemon=True).start()
%cd HRVC
clear_output()
print("Done Cloning Repository")
```
### Step 2: Install Requirements
Run the following commands to install all required packages:
```python
!pip install pip==23.3.1
!pip install -q -r requirements.txt
!pip install gradio-client==0.8.1
!pip install gradio==3.48.0
# install cuda fix
!python -m pip install ort-nightly-gpu --index-url=https://aiinfra.pkgs.visualstudio.com/PublicPackages/_packaging/ort-cuda-12-nightly/pypi/simple/
clear_output()
print("Finished Installing Requirements")
!sudo apt update
clear_output()
print("Finished Updating")
!sudo apt install sox
clear_output()
print("Finished running this cell, proceed to the next cell")
```
### Step 3: Download Models
Download the required MDXNet Vocal Separation and Hubert Base Models:

```python
models=codecs.decode('fep/qbjaybnq_zbqryf.cl','rot_13')
!python $models
clear_output()
print("Finished Downloading Voice Separation Model and Hubert Base Model")
```

### Step 4: Run the WebUI
Once the environment is set up, run the WebUI to start generating covers:

```python
runpice=codecs.decode('fep/jrohv.cl','rot_13')
!python $runpice --share
```

After running this, the Gradio URL will be generated. Simply click on the link and start creating your AI-powered cover art.

### Acknowledgments
This tool is based on [SociallyIneptWeeb's AICoverGen](https://github.com/SociallyIneptWeeb/AICoverGen). Special thanks to the developers for providing the original implementation.

### License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

```sql
This version of the README includes all necessary steps for setting up and running the AI-Cover-Generator, along with a clickable "Open in Colab" button.
```
