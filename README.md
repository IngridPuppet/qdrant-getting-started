# qdrant-getting-started-official

# Start Qdrant locally with docker

```bash
docker pull qdrant/qdrant
docker run -p 6333:6333 -p 6334:6334 \
  -v "$(pwd)/qdrant_storage:/qdrant/storage:z" \
  qdrant/qdrant
```

# Create and Load Mamba Environment from environment.yml

If you use [Mamba](https://mamba.readthedocs.io/en/latest/) for environment management, create and activate your environment from an `environment.yml` file with:

```bash
mamba env create -f environment.yml
mamba activate qdrant-getting-started-official
```

# Start Jupyter Lab

After activating your environment, launch Jupyter Lab with:

```bash
jupyter lab .
```
