Making a New Release
====================

 - create and upload a new github tag
 - version++ for 'version' and 'download url'

```python
 setup(
    # ...
    version='0.0.2',
    # ...
    download_url='https://github.com/TOPOI-DH/corpussearch/archive/0.0.2.tar.gz',
    )
```

 - add a github tag == version
 - run these commands:

```bash
python setup.py bdist_wheel --universal
python setup.py sdist
twine upload dist/*
```
