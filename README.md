# wXyEnginePy(WIP)

## Description

A tiny 2D game engine written in Python using ModernGL

It derived from my master thesis project.
It is currently under development and not ready for use.
I will add more functions as my project progresses.

## Structure

This engine is structured following JoltPhysics engine structure

It is divided into several modules:

- **Geometry**: contains the game object and primitives
- **Physics**: contains the physics classes
- **Rendering**: contains the rendering classes
- **Utils**: contains the utility classes

## Installation

##### PIP: Windows

```zsh
python3 -m venv venv
./venv/Scripts/activate.bat
pip install -r requirements.txt
```

##### PIP: Linux

```zsh
python3 -m venv venv
bash ./venv/bin/activate
pip install -r requirements.txt
```

##### Conda environment (recommended)

Install [miniconda](https://docs.conda.io/en/latest/miniconda.html) first.

```zsh
conda create -n wXyEngine-conda python=3.11 numpy scipy matplotlib
conda activate wXyEngine-conda
pip install del-msh imgui moderngl moderngl-window pygmsh
conda install pytorch torchvision torchaudio pytorch-cuda>=12.1 -c pytorch -c nvidia
conda install conda-forge::pygalmesh 
```

#### (Optional)Add and init as submodule

```zsh
git clone git@github.com:WvXY/wXyEnginePy.git
git submodule init
git submodule update
```

## TODO

- [ ] Add a proper README.md
- [ ] Rename class and submodule names to be more consistent
- [ ] Use only PyTorch
- [ ] Entity Component System
- [ ] Physics

## Black Formatting

I used the following options to format the code using black

```
--line-length=80 --preview
```

## References

- https://youtu.be/Y9U9IE0gVHA?si=kwfcpUtY0MACyFwI
- https://github.com/jrouwe/JoltPhysics/tree/master/Jolt
