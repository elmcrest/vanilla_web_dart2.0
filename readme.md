steps to reproduce the issue with non-relative packages, index.html is intentionally *not* inside of web.

Assuming Python 3.x and Dart 2.x is available:

1. clone repository
2. cd into it
3. pub get
4a. pub run build_runner watch -o js
4b. python3 -m http.server (new terminal window/tab)
5a. open `http://localhost:8000/js/web/some_static/index.html` and see 404 errors
5b. uncomment href tag in index.html to make example work, not really a solution to me...