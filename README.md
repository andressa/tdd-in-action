# TDD in Action (Django)

This git repo was created in order to practice TDD concepts using Python programming language.

It is based on [this book](http://www.obeythetestinggoat.com/book/).

## Primary Setup

After cloning the git repo, it is needed to create a conda environment and install requirements.

```bash
conda create -n tdd-in-action python=3

source activate tdd-in-action

pip install -r requirements.txt
```

```selenium``` package requires [```chromedriver```](https://chromedriver.storage.googleapis.com/index.html?path=2.29/) to execute functional tests. You should download it and moves it to your conda environment directory:

```bash
unzip ~/Downloads/chromedriver_OS.zip

mv ~/Downloads/chromedriver $ANACONDA/envs/tdd-in-action/bin
```

Above, you need to replace _OS_ by your current Operational System (in my case, I replaced by _mac64_).

Also, _$ANACONDA_ is an environment variable storing where _anaconda_ is installed.

## Running the project

To starting running Django server, just execute the following command line:

```bash
python manage.py runserver
```

## Running tests

### Functional tests

To run functional tests, you just need to execute the following command:

```bash
python functional_tests.py
```