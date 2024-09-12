## LLM4Psych_DGPS2024

This repository contains the materials for the DGPS 2024 pre-conference workshop, "Large language models in psychological research". The workshop introduces the use of open-source large language models (LLMs) from the Hugging Face ecosystem for research in psychology.

By [Zak Hussain](https://zak-hussain.github.io/) and [Dirk Wulff](https://www.mpib-berlin.mpg.de/person/93374/2549)

### Schedule

09:00 - 10:30: Talk: Introduction to large language models<br>
10:30 - 10:45: Break<br>
10:45 - 11:15: Talk: A gentle introduction to Hugging Face and Python<br>
11:15 - 11:45: Exercise:  Pipelines and APIs<br>
11:45 - 12:00: Walkthrough<br>
12:00 - 13:30: Lunch<br>
13:30 - 14:15: Talk: Intro to embeddings<br>
14:15 - 15:00 Exercise: Clarifying personality psychology<br>
15:00 - 15:15: Walkthrough<br>
15:15 - 15:45: Break<br>
15:45 - 16:15: Talk: Intro to text generation<br>
16:15 - 17:00: Exercise: Labeling and synthetic participants<br>
17:00 - 17:15: Walkthrough<br>
17:15 - 18:00: Discussion and Q&A<br>

### Additional Resources

<a href="https://doi.org/10.3758/s13428-024-02455-8">Hussain, Z., Binz, M., Mata, R., & Wulff, D. U. (2024). A tutorial on open-source large language models for behavioral science. *Behavior Research Methods*, 1-24.
</a>

Bibtex citation:

```
@article{hussain2024tutorial,
  title={A tutorial on open-source large language models for behavioral science},
  author={Hussain, Zak and Binz, Marcel and Mata, Rui and Wulff, Dirk U},
  journal={Behavior Research Methods},
  pages={1--24},
  year={2024},
  publisher={Springer}
}
```

[Hugging face documentation](https://huggingface.co/docs)<br>
[Hugging face book](https://transformersbook.com/)<br>
[But what is a GPT (3Blue1Brown)](https://www.youtube.com/watch?v=wjZofJX0v4M&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi&index=5)<br>

### Installation Instructions
0. If you do not have a Google account, you will need to create one (this can be deleted after the workshop).
1. Navigate to Google Drive (https://drive.google.com/).
2. In the top-left, click New > More > Colaboratory. If you do not see Colaboratory, you may need to click "Connect more apps", 
search for 'Colaboratory', and install it. Then click New > More > Colaboratory.
3. Copy the following code snipped into the first cell of the notebook. Run it (```shift + enter``` or click &#9658; button) to mount your Google Drive to the Colab environment.
A pop-up will ask you to connect; click through the steps to connect your Google Drive to Colab (you will have to do this
every time you open a new notebook).
```
from google.colab import drive
drive.mount("/content/drive")
```
4. Create a second cell in your notebook using the "+ Code" button that appears when you hover your cursor right under the first cell. Copy and run the following code snippet in the second cell of your notebook to clone the GitHub repository to your Google Drive :
```
%cd /content/drive/MyDrive
!git clone https://github.com/Zak-Hussain/LLM4Psych_DGPS2024.git
```
5. Go back to your Google Drive and navigate to the folder `LLM4Psych_DGPS2024`. You should see the relevant notebook (ending `.ipynb`) and data files in each folder (it may take  a couple of minutes for the files to appear).

#### Hugging Face API Setup Instructions
The following steps are required to access the Llama-3 model via the Hugging Face API, which we will use in the workshop.

6. Make sure you have a Hugging Face account (https://huggingface.co/join) (it's free!). 
7. Go to the [Llama-3 model page](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct) and fill in the 'META LLAMA 3 COMMUNITY LICENSE AGREEMENT' form at the top of the page in order to get access to the model (this can take up to an hour). 
8. Once you have received an email from Hugging Face saying that you have been granted access, you can navigate to [your Hugging Face profile settings](https://huggingface.co/settings/tokens) to generate an API access token. Click 'New token' at the bottom of the page, give your token a name, and select  'Type'='Read'. This token should provide access to all models in the Llama family. 
