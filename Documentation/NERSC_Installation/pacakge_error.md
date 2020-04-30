If you encouter following error:
```bash
ERROR: Could not install packages due to an EnvironmentError: [Errno 30] Read-only file system: '/global/common/cori_cle7/software/python/3.7-anaconda-2019.10/lib/python3.7/site-packages/corner-2.0.1.dist-info'
```
the chance is that NERSC got confused of installation directory. Try
```bash
which pip
```
If you get something like this:
```
/global/homes/k/kgb0255/.conda/envs/gqp/bin/pip
```
If not, NERSC is indeed confused because you might have done
```bash
module load python
```

If this is the case, close the shell and re-ssh to NERSC, and set up the environment **without** ```module load python```; i.e., 

```
#After you ssh into the NERSC server

conda create -n gqp python=3.7 ipython jupyter pip
which pip
```
and check if you get
```
/global/homes/k/kgb0255/.conda/envs/gqp/bin/pip
```

If not, feel free to contact us: kgb0255@berkeley.edu
