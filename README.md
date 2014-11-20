[![Build Status](https://travis-ci.org/ckan/ckan-service-provider.png?branch=master)](https://travis-ci.org/ckan/ckan-service-provider)
[![Coverage Status](https://coveralls.io/repos/ckan/ckan-service-provider/badge.png?branch=master)](https://coveralls.io/r/ckan/ckan-service-provider?branch=master)

[DataPusher]: https://github.com/okfn/datapusher


# CKAN Service Provier

__WORK IN PROGRESS__

A library for making web services that make functions available as synchronous
or asynchronous jobs. Used by [DataPusher][].


## Getting Started

To install ckanserviceprovider for development:

```bash
git clone https://github.com/ckan/ckan-service-provider.git
cd ckan-service-provider
pip install -r requirements-dev.txt
```

To get started making a web service with ckanserviceprovider have a look at
[/example](example). You can run the example server with
`python example/main.py example/settings_local.py`.

For a real-world example have a look at [DataPusher][].


## Running the Tests

To run the ckanserviceprovider tests:

```bash
nosetests
```


## Building the Documentation

To build the ckanserviceprovider docs:

```bash
python setup.py build_sphinx
```


## Releasing a New Version

To release a new version of ckanserviceprovider:

1. Increment the version number in [setup.py](setup.py)

2. Build a source distribution of the new version and publish it to
   [pypi.python.org](http://pypi.python.org/):

   ```bash
   python setup.py sdist
   ```

   You may want to test installing and running the new version from PyPI in a
   clean virtualenv before continuing to the next step.

3. Commit your setup.py changes to git, tag the release, and push the changes
   and the tag to GitHub:

   ```bash
   git commit setup.py -m "Bump version number"
   git tag 0.0.1
   git push
   git push origin 0.0.1
   ```

   (Replace both instances of 0.0.1 with the number of the version you're
   releasing.)


## Authors

The original authors of ckanserviceprovider were
David Raznick <david.raznick@okfn.org> and
Dominik Moritz <dominik.moritz@okfn.org>. For the current list of contributors
see [github.com/ckan/ckan-service-provider/contributors](https://github.com/ckan/ckan-service-provider/contributors)
