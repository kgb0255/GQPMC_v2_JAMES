Check if the existing symlinks are outdated by
```bash
cd $GQPMC_DIR
ls -l
```

Your symlinks should point to the proper directory; i.e. you should get
```bash
lrwxrwxrwx 1 kgb0255 kgb0255 42 Apr 23 17:30 Lgal -> /global/cfs/cdirs/desi/mocks/LGal_spectra/
lrwxrwxrwx 1 kgb0255 kgb0255 44 Apr 23 17:31 mini_mocha -> /global/cfs/cdirs/desi/mocks/gqp_mini_mocha/
lrwxrwxrwx 1 kgb0255 kgb0255 41 Apr 23 17:30 tng -> /global/cfs/cdirs/desi/mocks/TNG_spectra/
```

If they don't, discard the original symlinks and create new symlinks.
```bash
ln -s /global/cfs/cdirs/desi/mocks/LGal_spectra/ Lgal
ln -s /global/cfs/cdirs/desi/mocks/TNG_spectra/ tng 
ln -s /global/cfs/cdirs/desi/mocks/gqp_mini_mocha/ mini_mocha 
```
