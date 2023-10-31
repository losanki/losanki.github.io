---
layout: post
title: "Running tests before commit"
date: 2023-10-31 11:33:56 +0530
---

Running tests before commit

.git/hooks/pre-commit:

```
#!/bin/sh
echo “running tests before git commit”
. ./pre-tests.sh
```


pre-tests.sh:
```
#!/bin/sh

/Users/ravis/proj/brf/venv/bin/python manage.py test

if [ $? -ne 0 ]; then
 echo “tests failed”
 exit 1
fi
```
