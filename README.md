- Create environment from scratch
conda create -n agents python=3.11
conda activate agents
conda install -c conda-forge poetry
conda env export --from-history > environment.yml
- Create environment from file
conda env create -f environment.yml
- Run agent
langgraph dev
- Run fastapi server
fastapi dev app/api.py