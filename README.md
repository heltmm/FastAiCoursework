# Fast Ai Setup Rivanna UVA

### Installing

A guide to setup Fast Ai .7 for the 2018 Fast Ai course

commands to run in terminal:

username = your username
*need to use the uva vpn if off grounds

ssh into server
```
ssh username@rivanna1.hpc.virginia.edu
```
Clone git repo, move to that directory, create environment
```
git clone https://github.com/fastai/fastai.git
cd fastai
conda env create -f environment.yml
```
This may take some time

activate environment(conda or source depending on your version)
```
conda activate fastai
or 
source activate fastai
```

Installation is complete!

### Running

ssh into server
```
ssh username@rivanna1.hpc.virginia.edu
```

move to fastai and start environment
```
cd fastai
source activate fastai
```

start jupyter notebook
```
jupyter notebook
```
note your localhost port and token ex.

```
The Jupyter Notebook is running at:
http://localhost:8889/?token=eaeaafcd9e6ac1ff405ffdd45c59f60ea485e0f6a5631574
```
port:8889
token:eaeaafcd9e6ac1ff405ffdd45c59f60ea485e0f6a5631574

open new terminal tab

ssh into server with port forwarding
```
ssh -N -L localhost:8889:localhost:8889 username@rivanna1.hpc.virginia.edu
```
the first localhost is your machine and second is the rivanna server, my port 8888 was in use so used port 8889

go to http://localhost:8889 in your browser and when prompted enter your token.

Now you have your notebook up and running
