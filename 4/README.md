# HW4 setup
For this homework I needed to do a hacky work around to get mrjob to work. For
some reason, EMR does not like it when I run the mrjob script using python
3.5. To make the mrjob parts of Q4 work, create a virtual environment called
mrjob with [virtualenvwrapper](http://virtualenvwrapper.readthedocs.io/) like this:
```bash
mkvirtualenv -p /usr/bin/python2.7 mrjob
```
It should have activated the environment. If not, activate it with
`workon mrjob` and then run:
```bash
pip install -r https://raw.githubusercontent.com/SupaStuff/599_hw/master/4/requirements.txt
deactivate
```
Now you can run the notebook the usual way. In the parts where mrjob is
required, I have cells that activate this environment to run the script.
