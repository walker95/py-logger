# py-logger

Simple logger library for python. 

## Installation
Install the library
```
pip install git+https://github.com/walker95/py-logger.git
```

## Usage
```
#import the library
from py-logger import Logger, exception_logger
#setup logger
Logger = Logger()
logger = Logger.get_logger()
#print message
logger.info("this is a test message")
#for exceptions oneliners
try:
    1/0
except Exception:
    exception_logger(logger)
```
## Contributions
I just wanted to create a unified python logger that can simply generate oneline log records for log-forwarding services [fluent-bit, fluend, vector] to collection, formatting and forwarding. 

## License
MIT


