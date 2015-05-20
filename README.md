
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
