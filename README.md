# Benchmarking Python JSON serializers - json vs ujson vs orjson

If you work with a large datasets in json inside your python code, then you might want to try using 3rd party libraries like [ujson](https://github.com/ultrajson/ultrajson) and [orjson](https://github.com/ijl/orjson) which are replacements to python’s json library.

As per their documentation

- [ujson](https://github.com/ultrajson/ultrajson) (UltraJSON) is an ultra fast JSON encoder and decoder written in pure C with bindings for Python 3.7+.

- [orjson](https://github.com/ijl/orjson) is a fast, correct JSON library for Python. It is the fastest python library for json encoding & decoding. It serializes dataclass, datetime, numpy, and UUID instances natively.

## Benchmarking

OUTPUT:
Python 19.827091455459595
ujson 8.990580320358276
orjson 3.8100152015686035

## Conclusion

For most cases, you would want to go with python’s standard json library which removes dependencies on other libraries. On other hand you could try out [ujson](https://github.com/ultrajson/ultrajson) which is simple replacement for python’s json library. If you want more speed and also want dataclass, datetime, numpy, and UUID instances and you are ready to deal with more complex code, then you can try your hands on [orjson](https://github.com/ijl/orjson)
