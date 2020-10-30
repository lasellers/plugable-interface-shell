# plugable-interface-shell

This is something I have been mulling and posting about occasionally for a while.

The Cloud: This is a plugable adaptor to connect two apis, tools, etc through software that has in-memory caching and logging as well as input/output remapping. It is programming language and platform neutral.

In short, the interface shell is meant to minimize code in API or serverless apps, as well as remove language/framework specific request filtering and caching. Instead of defining caches in the API code or filters against the POST parms or GET, PUT, etc url args, etc and the various other JSON or encoded fields -- this is done with the interface shell itself. In YAML files. This way, we can minimize code in the API that has nothing to do with the actual operation it is created to handle.

Additionally: Am mulling plugable algorithms. That is to say, you can define various algorithms (for example, originally written using Python in Jupyter notebooks) but with a bash like interface allowing input/output to be chained. Through this, data from an API can be transformed through a series of prebuilt and well-tested functions. Increasing speed and reliability of automation setups.

Also: Acts as an private API Gateway.

Also: Caching has deterministic flags. That is, given the same set of input data, certain endpoints can be set to always return the result from the cache, if already computed. (Until the cache is refresh by other means/settings.) 
