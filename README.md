# important-script

# Set up Miniconda
Linux
```
mkdir -p miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O miniconda3/miniconda.sh
bash miniconda3/miniconda.sh -b -u -p miniconda3
rm -rf miniconda3/miniconda.sh
miniconda3/bin/conda init bash
miniconda3/bin/conda init zsh
```
# MAC
```
mkdir -p miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh  -O   miniconda3/miniconda.sh
bash miniconda3/miniconda.sh -b -u -p miniconda3
rm -rf miniconda3/miniconda.sh
miniconda3/bin/conda init bash
miniconda3/bin/conda init zsh
```
Install pyaudio for MAC
```
brew install portaudio
pip install --global-option='build_ext' --global-option='-I/usr/local/include' --global-option='-L/usr/local/lib' pyaudio
```
