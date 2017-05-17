nutroll
=======

This is a sample Python-language application intended to demonstrate connecting to Reddit via the [PRAW] library.

What you'll need to to start
----------------------------

1. Download and install [Python], if you haven't already.

2. Install the [PRAW] library. You may be able to do this with the administrator command ```pip install praw```.

3. [Create a "script" app on Reddit]. The "redirect uri" field can be ```http://localhost```.

4. Modify the ```nutroll``` file to include your Reddit app credentials:
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

Success:
```bash
$ ./nutroll your_reddit_username
Scanning for nut rolls (this may take several seconds)...
Nut roll detected: https://www.reddit.com/comments/6alu1h
```
Failure:
```bash
$ ./nutroll your_reddit_username
Scanning for nut rolls (this may take several seconds)...
No nut rolls this week.

```
PEBKAC:
```bash
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


    [PRAW]: https://github.com/praw-dev/praw
    [Python]: https://www.python.org/
    [Create a "script" app on Reddit]: https://www.reddit.com/prefs/apps
    [How do I use Git?]: http://git-scm.com/documentation
    [Download GitHub Desktop for Windows or Mac]: https://desktop.github.com/
    [Download Git for Linux]: http://git-scm.com/download/linux
