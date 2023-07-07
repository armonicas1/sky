# sky project

<p align="center"> <img src = "./streamlit/ressources/home.jpg"/ class="center"> </p>

<p>
This project, named sky, aims to detect and localize in satellite photos four 
specific types of cloud formations: Flower, Fish, Gravel and Sugar, so named because 
of their characteristic pattern.
</p>
<p>
The sky project is based on a 2019 <a href="https://www.kaggle.com/c/understanding_cloud_organization" 
target="new" rel="noopener noreferrer">Kaggle competition</a>, initiated by the Max Planck Institute. 
Main purpose was to mobilize the data scientist community on the realization of models capable of 
identifying shallow cloud locations, considered as potential key factors in climate’s understanding.
<br>
In this frame, we developed a convolutional neural network model trained to identify and localize the 
above four cloud formations.
<br>
More details on methodology and results are provided inside the article: <a href="https://towardsdatascience.com/silver-lining-clouds-with-ai-ff6a234786e2"> Silver-lining clouds with AI </a> published on Towards Data Science.

<p align="center"> <img src = "./resources/examples.jpg"/ class="center"> </p>


</p>

# Present repo content

<p>
The repository structure reflects project sequence. The sky project was organized in 3 phases: 
a first exploratory analysis, the second phase aimed at implementing a multi-classification model and the third one 
aimed at implementing a segmentation model. Libraries have also been developed and are grouped under the "packages" folder (associated documentation 
is available under "docPackages" folder).<br>
The 3 related jupyter notebook are visible from the «colab» links below.
</p>

# Explore the project

<p>To explore our work, just click the badges "Open In Colab" below.</p>
<ul type="circle">
<li>Explore phase 1 notebook in Google Colab (<i>sky_phase1_dataAnalyse.ipynb</i>)</li>
<p align="center"><a href="https://colab.research.google.com/github/DataScientest/sky/blob/master/sky_phase1_dataAnalyse.ipynb" target="new" rel="noopener noreferrer">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a></p>
<li>Explore phase 2 notebook in Google Colab (<i>sky_phase2_multiClassification.ipynb</i>)</li>
<p align="center"><a href="https://colab.research.google.com/github/DataScientest/sky/blob/master/sky_phase2_multiClassification.ipynb" target="new" rel="noopener noreferrer">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a></p>
<li>Explore phase 3 notebook in Google Colab (<i>sky_phase3_segmentation.ipynb</i>)</li>
<p align="center"><a href="https://colab.research.google.com/github/DataScientest/sky/blob/master/sky_phase3_segmentation.ipynb" target="new" rel="noopener noreferrer">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a></p>
</ul>
<p></p>

<p>Data in support to this work can be found below:</p>
<ul type="circle">
<li><a href="https://github.com/DataScientest/sky/tree/master/packages"> Library of functions and classes </a></li>
<li><a href="https://htmlpreview.github.io/?https://github.com/DataScientest/sky/blob/master/docPackages/index.html"> Library help </a></li>
</ul>

<p>Notes:</p>
<ul type="circle">
<li>Should nothing happen after a click, right-click the badge, then "open in new tab".</li>
<li>Google Colab will request access to your Github account on your first access.</li>
</ul>

# Streamlit application

<p>
This project resulted into a streamlit application intended to show the segmentation model in action. The sources of the application are available under the "streamlit" folder.
</p>
<p>
The streamlit application is available at:
<a href="https://studio.datascientest.com/project/sky/"> sky demo </a>.</p>

<p>Two possibilities enable to test your own version of the application:
</p>
<p><b>Launch Streamlit from sources through Google Colab:</b><br>
<i>Note: a Ngrok account is required.</i></p>
<p align="center"><a href="https://colab.research.google.com/github/DataScientest/sky/blob/master/sky_demo_streamlitColab.ipynb" target="new" rel="noopener noreferrer">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a></p>
<p><b>Or, install sky Streamlit application:</b></p>

<p>Here is an example for RPM-based distributions.<br>
<ul type="circle">
 <li>Install Streamlit:</li>
  <p><i>python3 -m pip install streamlit</i></p> 
 <li>Install git:</li>
  <p><i>sudo yum upgrade<br>
        sudo yum install git</i></p>
 <li>Clone sky repo:</li>
  <p><i>git clone https://github.com/DataScientest/sky</i></p>
 <li>Install requirements:</li>
  <p><i>cd sky<br>
        python3 -m pip install opencv-python-headless<br>
        python3 -m pip install --no-cache-dir tensorflow<br>
        python3 -m pip install scikit-learn<br>
        pip install -r streamlit/requirements.txt</i></p>
 <p>When launching the demo in both mode (runtime or tmux), 
     please run the app as mentioned below to get dark theme active.</p>
 <li>Launch runtime session:</li>
  <p><i>cd streamlit<br>
        streamlit run index.py</i></p>
 <li>Or launch tmux session:</li>
  <p><i>cd streamlit<br>
        tmux new -s st_instance<br>
        streamlit run index.py</i></p>

# Credits

<p>
The project sky was carried out as student project for Data Scientist training course at the DataScientest institute <a href="https://datascientest.com">(datascientest.com)</a> </p>

<p><u>Project members:</u><br>
<a href="https://www.linkedin.com/in/hans-schauer-454324235/" target="new" rel="noopener noreferrer">
Hans Schauer <img src="./streamlit/ressources/linkedin.png" width=20px alt="Hans Schauer"/></a><br>
<a href="https://www.linkedin.com/in/hans-schauer-454324235/" target="new" rel="noopener noreferrer">
Georg Wolf <img src="./streamlit/ressources/linkedin.png" width=20px alt="Georg Wolf"/></a></p>

<p><u>Project mentor:</u><br>
<a href="https://www.linkedin.com/in/hans-schauer-454324235/" target="new" rel="noopener noreferrer">
Victor (DataScientest) <img src="./streamlit/ressources/linkedin.png" width=20px alt="Victor (DataScientest) "/></a></p>
