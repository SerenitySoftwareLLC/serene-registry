CahootsRegistry
===============

A simple, non-persistent, key-value registry in memory.

Contributors
------------
1. [Ryan Vennell] (https://github.com/hickeroar)

Installation
------------

`sudo pip install CahootsRegistry`

Usage
-----

```
from CahootsRegistry import registry

# statically saves the value '1234' into the key 'foo'
# You can now import the registry module from another class and access foo there.
registry.set("foo", 1234)

# returns 1234
registry.get("foo")

# returns None
registry.get("bar")

# returns True 
registry.test("foo")

# returns False
registry.test("bar")

# empties all values from the registry
registry.flush()

# You can access the data directly as well
registry.storage['foo']
```
