wget https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-MacOSX-arm64.sh
ls
bash Mambaforge-MacOSX-arm64.sh
cd mambaforge
ls
cd etc
ls
cd profile.d
ls
source conda.sh
conda install -yq mamba
mamba install pytorch::pytorch torchvision torchaudio -c pytorch
mamba install jupyterlab
mamba install ipython
mamba install ipywidgets
mamba install fastcore
mamba list
echo $PATH
mamba install -c fastai fastai
mamba install -c fastchan fastbook
mamba install -c fastchan sentencepiece
mamba install -c fastai -y nbdev
mamba list
mamba install fastcore
mamba install fastdownload
mamba install pandas
mamba install numpy
mamba install sympy
mamba install kaggle
mamba install seaborn
mamba install sklearn
mamba install graphviz
mamba install fastcore
pip install -Uq fastkaggle
mamba install plotly
mamba install scikit-learn
mamba install matplotlib
mamba install opencv
mamba install bs4
mamba install nltk
mamba install openpyxl
mamba install wordcloud
mamba repoquery whoneeds fastai
mamba config list --sources
mamba info
type -a python
mamba install transformers
mamba install datasets
mamba install pipelines
mamba install pipeline
mamba install tqdm
mamba install wandb
mamba install peft
mamba install accelerate
mamba install evaluate
mamba install backoff
mamba install nbformat
mamba install execnb
ls
ls -a
bbedit .zshrc
bbedit .zsh_history
