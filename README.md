# MGDT term project

## Quickstart
```bash
conda env create -f conda_env_1.yml
conda activate mgdt_1
pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 -f https://download.pytorch.org/whl/torch_stable.html
pip install -r requirements.txt
pip install dopamine-rl
pip install "gymnasium[atari, accept-rom-license]”


python scripts/download_weights.py
python run.py
```
## Dataset
```bash
mkdir [DIRECTORY_NAME]
gsutil -m cp -R gs://atari-replay-datasets/dqn/[GAME_NAME] [DIRECTORY_NAME]
```

## References:

- [1] Original code in Jax: https://github.com/google-research/google-research/tree/master/multi_game_dt
- [2] Paper: https://arxiv.org/abs/2205.15241
