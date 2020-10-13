DANCE: Difficulty and Novelty Co-Driven Exploration
Our code is based on RND (https://github.com/openai/random-network-distillation) and Openai baselines (https://github.com/openai/baselines).


### Installation and Usage
The env you need install:
python 3.6
CUDA 10.0
CUDNN 7.6.0
pip install gym
pip install gym[atari]
pip install tensorflow-gpu==1.14.0
pip install numpy
openmpi
pip install mpi4py

The following command should train an DANCE agent on Montezuma's Revenge

python run_atari.py --gamma_ext 0.999

To use more than one gpu/machine, use MPI (e.g. `mpiexec -n 8 python run_atari.py --num_env 128 --gamma_ext 0.999` should use 1024 parallel environments to collect experience on an 8 gpu machine). 


