<p align="center">
  <h3 align="center">Example to RAML</h3>

  <p align="center">
    Creates a draft RAML specifications file from existing log file or strings.
  </p>
</p>
<br>
The normal way of things is to create the RAML API documentation file and then implement the code. However, sometimes we need to document an existing API. The software in this repository is intended to make this task much less painful, by automatically generating a part of the RAML file. Of course, you will still need to fix and enhance the file afterwards.


## Table of contents

- [Quick start](#quick-start)
- [Overview](#overview)
- [Prerequisites and Installing](#prerequisites-and-installing)
- [Author](#author)
- [License](#license)

## Quick start

### By Importing an existing log file

In order to generate the draft .raml file, simply run this software, giving it the log file name as a parameter.
NOTE: Not implemented yet

### By specifying parameters and/or response strings

A more basic use is to run the software without filename as a parameter. In such case, the software will prompt for a Json (or YAML) parameters string containing dictionary and a similar response string. Those two strings will be converted to the appropriate sections of the RAML file.
The strings are expected to be a valid JSON dictionary, with some relaxations. 

## Overview

The basic process done is to look for URLs and assume those are requests and for curlies, and assume those are the parameters and/or replies.
The software will also try to detect whether the log was produced by Jave/JavaScript or by Python.## Prerequisites and Installing

Python 3.x is needed.
You can get and install Python from the [Python Software Foundation](https://www.python.org/) 

No other installation is needed. Just get the repository.


## Author

**Shalom Mitz** - [shalommmitz](https://github.com/shalommmitz)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

