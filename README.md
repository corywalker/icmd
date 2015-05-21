
```
usage: icmd [-h] [-s] [-n NUMBER] [-l LIMIT] [-b BUDDY] [-m MSG] [--first]
            [-d]

Command line interface to OSX Messages

optional arguments:
  -h, --help            show this help message and exit
  -s, --send            Set to send mode rather than check mode (default:
                        check)
  -d, --debug           Debug mode. Do not actually send any messages, print
                        commands instead. (default: False)

MODE: Checking (default):
  -n NUMBER, --number NUMBER
                        Number of messages to grab, newest first (default: 50)
  -l LIMIT, --limit LIMIT
                        Max number of messages to display per buddy (default:
                        None)

MODE: Sending:
  -b BUDDY, --buddy BUDDY
                        Buddy to send message to. Name matches against
                        displayed name or number. (default: None)
  -m MSG, --msg MSG     Message to send. Will prompt if not provided.
                        (default: None)
  --first               Noninteractive send. Send to the first matching buddy.
                        CAN CAUSE SENDING TO UNINTENTIONAL BUDDIES. (default:
                        False)
```

Install:
--------

This is just a single script in the `bin` folder. Simply clone the repository and run it as you wish.

Examples:
---------

```
{19:46}~ ➭ icmd
BRANDON KELCEY:
05-20 19:15:07  < At the football game!

CHARLIE MCGUIRE:
05-20 19:19:24 > OK you can text but don't call - in the library
05-20 19:19:28 > What are you up to tonight?
05-20 19:22:02  < Not sure - I'm going to the game first
05-20 19:23:54 > Sounds good. we should hang out after
```

```
{19:54}~ ➭ icmd -s -b charlie
CHARLIE MCGUIRE:
05-20 19:19:24 > OK you can text but don't call - in the library
05-20 19:19:28 > What are you up to tonight?
05-20 19:22:02  < Not sure - I'm going to the game first
05-20 19:23:54 > Sounds good. we should hang out after

Message to send: absolutely!
```
