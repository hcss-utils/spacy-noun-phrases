# spacy-phrases

This repository contains spacy-based **`noun-phrases extraction`** script. 

## Usage

To use or contribute to this repository, first checkout the code. 
Then create a new virtual environment:

```console
$ git clone https://github.com/hcss-utils/spacy-phrases.git
$ cd spacy-phrases
$ python3 -m venv env
$ . env/bin/activate
$ pip install -r requirements.txt
```

To extract phrases, run `python scripts/main.py`: 

```console
Usage: main.py [OPTIONS] INPUT_TABLE OUTPUT_JSONL

  Extract noun phrases using spaCy.

Arguments:
  INPUT_TABLE   [required]
  OUTPUT_JSONL  [required]

Options:
  --model TEXT                    [default: en_core_web_sm]
  --text-field TEXT               [default: fulltext]
  --uuid-field TEXT               [default: uuid]
  --pattern TEXT                  [default: influenc]
  --install-completion [bash|zsh|fish|powershell|pwsh]
                                  Install completion for the specified shell.
  --show-completion [bash|zsh|fish|powershell|pwsh]
                                  Show completion for the specified shell, to
                                  copy it or customize the installation.
  --help                          Show this message and exit.
```

To count phrases, see [`notebooks/count-phrases.ipynb`](notebooks/count-phrases.ipynb)