# Filter Lines Through An External Program

Vim allows you to search and replace using regex. Using an index, you can
place part of the existing content where you want it.

```
:%s/"{{ STATIC_URL }}\/\(.*\)"/"{% static '\1' %}"/gc
```


See `http://vim.wikia.com/wiki/Search_and_replace` for more details.
