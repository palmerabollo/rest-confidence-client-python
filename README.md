rest-confidence-client-python
=============================

This is a Python client for the simple [rest-confidence configuration server](https://github.com/palmerabollo/rest-confidence).

This is not rocket science, but it hides the REST API details if you do not want to worry about them.

Usage
-----

Instantiate a ConfigurationResolver

```
resolver = ConfigurationResolver('http://localhost:8000', {env: 'development'});
```

and use it:

```
resolver.load();
resolver.load('key1');
resolver.load('key2/limit');
```

License
-------

MIT
