# MaxiGauge

This is a software written in Python to log vacuum pressure values
from a Pfeiffer-Vacuum MaxiGauge vacuum gauge controller.

It is capable of displaying vacuum pressure values live on
the web and logging them to a file.

## Requirements

* [Python][] (works with 2.7 and >= 3)
* [PySerial][] to communicate with the MaxiGauge via the RS232 port.
* [PyYAML][] to load settings from yaml file.
* [Bottle][] to start the web server.
* [CherryPy][] to use as a different web server.

## Getting started

1. install the dependencies: `python -m pip install -r requirements.txt` (
   or `python3 -m pip install -r requirements.txt` if you're using python3 explicitly)
2. change port and logfile name in [settings.yml][] to the appropriate values
3. (optional) change the desired webserver at the bottom of [webserver.py][]
4. start the server: run `./webserver.py` (or `python webserver.py` or `python3 webserver.py` to specify a version)

## License

Copyright (C) 2012 Philipp Klaus (Institut fuer Kernphysik Frankfurt)

The following license only applies to files written by Philipp Klaus.
A couple of other files have different licenses, such as the javascript
libraries d3, Rickshaw, jQuery and cubism!

> Permission is hereby granted, free of charge, to any person
> obtaining a copy of this software and associated documentation files
> (the "Software"), to deal in the Software without restriction, including
> without limitation the rights to use, copy, modify, merge, publish,
> distribute, sublicense, and/or sell copies of the Software, and to
> permit persons to whom the Software is furnished to do so, subject to
> the following conditions:
>
> The above copyright notice and this permission notice shall be
> included in all copies or substantial portions of the Software.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
> EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
> MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
> IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
> CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
> TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
> SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[Python]: http://www.python.org/getit/

[PySerial]: https://pypi.org/project/pyserial/

[PyYAML]: https://pyyaml.org/

[Bottle]: http://bottlepy.org

[CherryPy]: https://cherrypy.dev/

[settings.yml]: settings.yml

[webserver.py]: webserver.py