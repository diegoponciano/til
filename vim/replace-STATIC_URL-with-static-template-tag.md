# Replace STATIC_URL with {% static %} template tag

Vim allows you to search and replace using regex. Using an index, you can
place part of the existing content where you want it.

```
:%s/"{{ STATIC_URL }}\/\(.*\)"/"{% static '\1' %}"/gc
:%s/"{{ STATIC_URL }}\/\(.\{-}\)\"/"{% static '\1' %}"/c"
```


See `http://vim.wikia.com/wiki/Search_and_replace` and `:help /\{-` for more details.
