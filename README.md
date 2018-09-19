[![Build Status](https://travis-ci.org/chrisjsewell/aiida-gulp.svg?branch=master)](https://travis-ci.org/chrisjsewell/aiida-gulp) 
[![Coverage Status](https://coveralls.io/repos/github/chrisjsewell/aiida-gulp/badge.svg?branch=master)](https://coveralls.io/github/chrisjsewell/aiida-gulp?branch=master) 
[![Docs status](https://readthedocs.org/projects/aiida-gulp/badge)](http://aiida-gulp.readthedocs.io/) 
[![PyPI version](https://badge.fury.io/py/aiida-gulp.svg)](https://badge.fury.io/py/aiida-gulp)

# aiida-gulp

AiiDA plugin for use with GULP

Templated using the [AiiDA plugin cutter](https://github.com/aiidateam/aiida-plugin-cutter).

## Installation

```shell
git clone https://github.com/chrisjsewell/aiida-gulp .
cd aiida-gulp
pip install -e .  # also installs aiida, if missing (but not postgres)
#pip install -e .[pre-commit,testing] # install extras for more features
verdi quicksetup  # better to set up a new profile
verdi calculation plugins  # should now show your calclulation plugins
```

## Usage

Here goes a complete example of how to submit a test calculation using this plugin.

A quick demo of how to submit a calculation:
```shell
verdi daemon start         # make sure the daemon is running
cd examples
verdi run submit.py        # submit test calculation
verdi calculation list -a  # check status of calculation
```

If you have already set up your own aiida_gulp code using `verdi code setup`, you may want to try the following command:
```
gulp-submit  # uses aiida_gulp.cli
```

## Tests

The following will discover and run all unit test:
```shell
pip install -e .[testing]
python manage.py
```

## License

MIT


## Contact

chrisj_sewell@hotmail.com
