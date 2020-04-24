If you encounter this:

```bash
ERROR: Command errored out with exit status 1:
     command: /global/homes/k/kgb0255/.conda/envs/gqp/bin/python -c 'import sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-t3rettln/multiprocessing/setup.py'"'"'; __file__='"'"'/tmp/pip-install-t3rettln/multiprocessing/setup.py'"'"';f=getattr(tokenize, '"'"'open'"'"', open)(__file__);code=f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-install-t3rettln/multiprocessing/pip-egg-info
         cwd: /tmp/pip-install-t3rettln/multiprocessing/
    Complete output (6 lines):
    Traceback (most recent call last):
      File "<string>", line 1, in <module>
      File "/tmp/pip-install-t3rettln/multiprocessing/setup.py", line 94
        print 'Macros:'
                      ^
    SyntaxError: Missing parentheses in call to 'print'. Did you mean print('Macros:')?
    ----------------------------------------
ERROR: Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.
```

Neglect it.

https://stackoverflow.com/questions/42568638/python-multiprocessing-installation-command-python-setup-py-egg-info-failed-w
