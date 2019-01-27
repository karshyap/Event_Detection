# Open-Domain Event Detection using Distant Supervision

This repository provides a dataset used in our [COLING 2018
paper](http://junaraki.net/pubs/coling2018-event.pdf) titled ``Open-Domain
Event Detection using Distant Supervision.''  The dataset comprises 100 Simple
English Wikipedia articles in 10 different domains, annotated with events.  We
call the dataset SW100.  We also provide our code for the rule-based event
detection system (RULE) described in the paper.

## Requirements
- Python 3.6
- Java 8

For other requirements on python packages, please look at ```requirements.txt```.

## How to Run the Code
```
$ sh download.sh
$ sh preprocess.sh
$ python wsd.py
$ python phrase.py
$ python rule.py
$ python ann2brat.py
```

Running `wsd.py` (word sense disambiguation) may take several hours.  If you
can successfully run the code, you should be able to get system output in the
[Brat standoff format](http://brat.nlplab.org/standoff.html) under `out/SW100`.


## Citation
If you use the dataset and/or the code, please cite our COLING 2018 paper:

```
@inproceedings{Araki2018OpenDomain,
  author    = {Jun Araki and Teruko Mitamura},
  title     = {Open-Domain Event Detection using Distant Supervision},
  booktitle = {Proceedings of COLING},
  month     = {August},
  year      = {2018},
  address   = {Santa Fe, NM, USA},
}
```
