nutroll
=======

This is a sample Python-language application intended to demonstrate connecting to Reddit via the [PRAW] library.

What you'll need to to start
----------------------------

* Download and install [Python], if you haven't already.

* Install the [PRAW] library (You may be able to do this with the administrator command ```pip install praw```).

* [Create a "script" app on Reddit] (The "redirect uri" field can be ```http://localhost```).

* Modify the ```nutroll``` file to include your Reddit app credentials:
```python
return praw.Reddit(
  client_id='mHJAei1MCbztxw',
  client_secret='G74uVCX9K5MnyBcNhDFwpwqVZtY',
  #...
)
```

Where the ```client_id``` and ```client_secret``` are obtained from your Reddit app settings.

Example of running the ```nutroll``` application:
----------------------------------------------------

* Success:
```
$ ./nutroll your_reddit_username
Scanning for nut rolls (this may take several seconds)...
Nut roll detected: https://www.reddit.com/comments/6alu1h
```
* Failure:
```
$ ./nutroll your_reddit_username
Scanning for nut rolls (this may take several seconds)...
No nut rolls this week.

```
* PEBKAC:
```
$ ./nutroll your_reddit_username
Scanning for nut rolls (this may take several seconds)...
Unable to reach Reddit. Did you setup your credentials properly?

```


Additional resources
--------------------

* [How do I use Git?]

* [Download GitHub Desktop for Windows or Mac]

* [Download Git for Linux]

* http://en.wikipedia.org/wiki/Git_(software)


About
-----

nutroll was developed by [Greg M. Krsak] using [PyCharm] Community 2017.1 on [Linux Mint] 18.1.

Please submit bugs to [the issues page] and feel free to contribute pull requests.

  [PRAW]: https://github.com/praw-dev/praw
  [Python]: https://www.python.org/
  [Create a "script" app on Reddit]: https://www.reddit.com/prefs/apps
  [How do I use Git?]: http://git-scm.com/documentation
  [Download GitHub Desktop for Windows or Mac]: https://desktop.github.com/
  [Download Git for Linux]: http://git-scm.com/download/linux
  [Greg M. Krsak]: https://github.com/gregkrsak
  [PyCharm]: https://www.jetbrains.com/pycharm/
  [Linux Mint]: https://linuxmint.com/
  [the issues page]: https://github.com/gregkrsak/nutroll/issues

