**2021-10-08**

Just set up repository, somewhere to jot notes (here) - transfer into README when there's a bit of code to show...

Motivation, mostly to help with NewsMonitor blogroll, but should be handy elsewhere.

Soo...

## Initial Requirements

- read file containing a list of URLs
- do a HTTP GET on each
- capture the status
- if the status is on filter list (eg 200 OK), add the URL to a list
- save list to file

Probably a initial good default would be to call 1xx, 2xx, 3xx _good_, 4xx, 5xx _bad_. Channel to two simple list text files.

## Implementation

I want to have a play with [Javascript Promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) and it might be convenient to have this thing running standalone in a browser.

https://web.dev/promises/

https://web.dev/async-functions/

https://tc39.es/ecma262/#sec-promise-objects

https://github.com/domenic/promises-unwrapping/blob/master/docs/states-and-fates.md

But initially command line to keep things simple.

Hmm..maybe have a play in a Jupyter Notebook...

Already had [Jupyter Notebook](https://jupyter.org/) installed, added the [ijavascript kernel](https://github.com/n-riesco/ijavascript) (uses node.js).

## Status Codes

([Wikipedia](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes))

- 1xx informational response – the request was received, continuing process
- 2xx successful – the request was successfully received, understood, and accepted
- 3xx redirection – further action needs to be taken in order to complete the request
- 4xx client error – the request contains bad syntax or cannot be fulfilled
- 5xx server error – the server failed to fulfil an apparently valid request

## Later

- figure out redirects - replace URL as appropriate
- input/output in Turtle
- specify filter in Turtle
