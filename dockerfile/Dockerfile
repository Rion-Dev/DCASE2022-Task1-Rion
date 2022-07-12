FROM nvidia/cuda:11.2.1-devel-ubuntu20.04
RUN apt-get update && apt-get install -y \
sudo \
wget \
vim

RUN apt-get update

RUN apt-get install -y python3 python3-pip

RUN apt-get install git -y

RUN pip install --upgrade pip

RUN pip install jupyterlab

RUN pip install jupyterlab-git

RUN pip install torch==1.11.0+cu113 torchvision==0.12.0+cu113 torchaudio==0.11.0+cu113 -f https://download.pytorch.org/whl/cu113/torch_stable.html

RUN pip install pandas 
RUN pip install matplotlib
RUN pip install tqdm
RUN pip install livelossplot
RUN pip install tensorflow
RUN pip install torchinfo

WORKDIR /
CMD ["jupyter","lab","--ip=0.0.0.0","--allow-root","--LabApp.token=''"]

