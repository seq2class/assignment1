# Assignment 1

## Getting started
Instructions for the tasks are included in the jupyter notebook, run `jupyter
notebook` once you have setup your environment.

## Installing
For all of our assignments, we will be using [anaconda](https://www.anaconda.com/download/) with python 3.7 and [pytorch](http://pytorch.org/).

Download anaconda from [here](https://www.anaconda.com/download/), and then you can install pytorch by running: `conda install pytorch-cpu -c pytorch`.  You can then launch the Jupyter notebook by running: `jupyter notebook`

On Linux this looks like:
```bash
curl -O 'https://repo.anaconda.com/archive/Anaconda3-2018.12-Linux-x86_64.sh'
bash Anaconda3-2018.12-Linux-x86_64.sh
source ~/anaconda3/bin/activate
conda install pytorch-cpu -c pytorch
jupyter notebook
```

### Using an ugrad machine
If you are unable to get python working on your local computer or would rather
use the ugrad machines to work on your homework, then you can follow these
instructions:

```bash
# replace 1234 with your favorite number
ssh USERNAME@ugrad10.cs.jhu.edu -L 1234:localhost:1234
curl -O 'https://repo.anaconda.com/archive/Anaconda3-2018.12-Linux-x86_64.sh'
bash Anaconda3-2018.12-Linux-x86_64.sh
bash
source ~/anaconda3/bin/activate
conda install pytorch-cpu -c pytorch
jupyter notebook --ip=127.0.0.1 --port=1234 --no-browser
```

Now open your web browser to `http://localhost:1234` and you should see the jupyter notebook login screen.
If it is asking you for a token, then check the output in the terminal for a line like:
```
Copy/paste this URL into your browser when you connect for the first time,
to login with a token:
    http://127.0.0.1:9001/?token=a552f07a9b00cc2b84f
```

## Submitting your assignment:
  1. Make sure that you have completed all parts of the assignment
  2. In the Jupyter notebook click **Kernel > Restart & Run all** to generate the output for all cells
  3. Save the notebook *with* the output from all the cells in the notebook **File > Save and Checkpoint**
  4. Upload the .ipynb file to Piazza (you should not need to upload anything else for this assignment)
