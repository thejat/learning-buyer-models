### Code for the paper "An Online Algorithm for Learning Buyer Behavior under Realistic Pricing Restrictions"

This codebase is for algorithms proposed in the aforementioned [paper](https://arxiv.org/abs/1803.01968). It consists of four python scripts:

  * algorithms.py : has the proposed and competitor algorithms
  * data.py : generates data (e.g., from the billion prices project)
  * experiments.py : (calls algorithms on buyer models)
  * buyers.py : has the four buyer models
  * geometric.py : has definitions for primitives such as ellipsoids and halfspaces that are used in the algorithms.

The easiest way to get started is to look at experiments.py and go from there.

###### Some useful pointers:

To reload Ipython modules (useful for debugging) following [this](https://stackoverflow.com/questions/5364050/reloading-submodules-in-ipython):

```python
%load_ext autoreload
%autoreload 2
```

This can be saved in `~/.ipython/profile_default/ipython_config.py` as

```python
c.InteractiveShellApp.extensions = ['autoreload']     
c.InteractiveShellApp.exec_lines = ['%autoreload 2']
```
