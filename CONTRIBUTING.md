Making a New Release
====================

 - create and upload a new github tag == version
 - version++ for 'version' and 'download url'

```python
 setup(
    # ...
    version='0.0.2',
    # ...
    download_url='https://github.com/computational-antiquity/corpussearch/archive/0.0.2.tar.gz',
    )
```

 - run these commands:

```bash
python setup.py sdist bdist_wheel
twine upload dist/*
```
