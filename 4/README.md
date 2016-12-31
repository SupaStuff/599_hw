# HW4 setup
For this homework I needed to do a hacky work around to get mrjob to work. For
some reason, EMR does not like it when I run the mrjob script using python
3.5. To make the mrjob parts of Q4 work, create a virtual environment called
mrjob with virtualenvwrapper like this:
```bash
mkvirtualenv -p /usr/bin/python2.7 mrjob
```
It should have activated the environment. Navigate to this directory and run:
```bash
pip install -r requirements.txt
deactivate
```
Now you can run the notebook the usual way. In the parts were mrjob is
required, the cells will activate this environment to run the script.
