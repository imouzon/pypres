#Installing Python on a mac
There are two main versions of Python, `Python 3.x` and `Python 2.x`.
The conversation over which one is preferable seems to be
occurring mainly on the side of development using Python
(apparently, it is very easy to create GUI apps using a few key Python
tools) but it boils down to this (my understanding):
* Python 3 is the future of Python and we should try to use it as our default
and
* Python 3 will break your computer because everything special about Python still depends on Python 2
this of course means that you should install both of them. 
It actually seems like there is more to it than that, as can be seen by reading
the subtext in the [main discussion](https://wiki.Python.org/moin/Python2orPython3) on the Python wiki about how to choose between
the two. 
It seems like there is a lot of frustration on the part of the `Python 3` people.

Of course, you should install both.

##Homebrew
I have used a few package managers (macports and fink primarily). 
Homebrew is the best I have used so far, mainly because I mostly understand it.
However, it also has a healthy future (In 2013, according to Wikipedia, Homebrew
had the largest number of contributers on Github).

###Installing Homebrew
You do not have to install Xcode. 
Xcode is large and outside of the scope of what we usually do in statistics.
All you really need is the `Command Line Tools` which can be acquired by using

```Shell
xcode-select --install
```

and we can then install Homebrew:

```Shell
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
The Homebrew directory should be added to your path (I think this may occur automatically).
Simply open a file in `~/.profile` and add the line
```Shell
export PATH=/usr/local/bin:/usr/local/sbin:$PATH
```

##Installing python
First check the version of Python you are using:
```Shell
python --version
```
This will report that the command `python` could not be found if you do not have any
version of python on your machine.
Also, check the version of Python 3:
```Shell
python3 --version
```
If you aren't using Python 2.7, do the following:
```Shell
brew install python
```
and Python 3.4 seems to be the going version of Python 3:
```Shell
brew install python
```
You are now ready to run Python 2:
```Shell
python
```
or Python 3:
```Shell
python3
```

##Writing Python code
Now that we have Python frameworks installed, we can start running code.
For those of you who feel most comfortable in Rstudio, I recommend [Spyder](https://code.google.com/p/spyderlib/)
which seems to be the most "R like" coding environment for python.

(I will do a brief demonstration if I have time).
