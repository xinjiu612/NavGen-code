# NavGen

Visual Generative Models as a Scalable Data Engine for Embodied 3D Navigation.

## Description

NavGen contains first-person navigation videos with detailed action descriptions (prompts). Each sample is a short video clip paired with a prompt describing the scene and camera motion.

## Download

### HuggingFace

Data: https://huggingface.co/datasets/xinjiu/NavGen

Install dependencies:

```bash
pip install datasets huggingface_hub
```

Download via Python:

```bash
python -c "from datasets import load_dataset; dataset = load_dataset('xinjiu/NavGen')"
```

Or via huggingface_hub CLI:

```bash
huggingface-cli download xinjiu/NavGen --repo-type dataset --local-dir ./NavGen
```

Or via git clone:

```bash
git lfs install
git clone https://huggingface.co/datasets/xinjiu/NavGen
```

### ModelScope

Data: https://www.modelscope.cn/datasets/xinjiu612/NavGen

Install dependencies:

```bash
pip install modelscope
```

Download via Python:

```bash
python -c "from modelscope import snapshot_download; snapshot_download('xinjiu612/NavGen', repo_type='dataset', local_dir='./NavGen')"
```

Or via CLI:

```bash
modelscope download --dataset xinjiu612/NavGen --local_dir ./NavGen
```

> Note: You may need to set your ModelScope API token first.

## Files

- `NavGen.csv`: video filenames and prompts.
- `navgen_videos.tar.gz`: packed video files.

We will release all our datasets and models once the paper is accepted.
