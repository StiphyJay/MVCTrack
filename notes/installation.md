## Installation

Below are the key dependencies for running MVCTrack:

| Dependency | Version  |
|------------|----------|
| Python     | 3.9.0    |
| PyTorch    | 2.0.1    |
| MMEngine   | 0.7.4    |
| MMCV       | 2.0.0    |
| MMDet      | 3.0.0    |
| MMDet3D    | 1.1.0    |
| SpConv     | 2.3.6    |
| YAPF       | 0.40.0   |

---

## Preparation

Clone the repository to your local directory:

git clone https://github.com/StiphyJay/MVCTrack.git

We recommend using conda to manage the environment.

### Step 1: Create and activate a new conda environment

conda create -n mvc python=3.9
conda activate mvc

### Step 2: Install the key dependencies

- Install PyTorch and related libraries:

`pip install torch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 --index-url https://download.pytorch.org/whl/cu118`

- Install MMCV:

`pip install mmcv==2.0.0 -f https://download.openmmlab.com/mmcv/dist/cu118/torch2.0/index.html`

- Install SpConv:

`pip install spconv-cu118==2.3.6`

### Additional Notes

- Ensure your system has CUDA 11.8 installed to match the dependencies listed above.
- Other dependencies like MMEngine, MMDet, MMDet3D, and YAPF will be installed automatically when running the setup or can be installed manually using pip.
- For detailed instructions on environment setup, please refer to the project documentation.

### Step 3: Install segmentor CenterNet2

Please install [CenterNet2](https://github.com/xingyizhou/CenterNet2). 
Make sure to add a link to [CenterNet2](https://github.com/xingyizhou/CenterNet2/tree/master/projects/CenterNet2) folder in your Python path.
We will use CenterNet2 for 2D instance segmentation and use the segmentation results to generate the virtual points.
