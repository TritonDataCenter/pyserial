# Joyent pyserial 3.4

This fork of pyserial 3.4 exists so that some rather trivial changes
can be made to support Python 2.6.  This is needed for cloud-init on
Centos 6 when running in bhyve on SmartOS.

## To build the rpm

Check out this branch, then:

```
$ python setup.py bdist_rpm
```

You will find the rpm and source rpm in the `dist` directory.  In the
event that this ever gets rebuilt, you will want a new version number.
See https://docs.python.org/2.0/dist/creating-rpms.html for more details.
