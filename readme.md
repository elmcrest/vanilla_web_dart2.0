steps to reproduce the issue with non-relative packages, index.html is intentionally *not* inside of web.

Assuming Python 3.x and Dart 2.x is available:

1. `git clone` repository
2. `cd` into it
3. `pub get`
4. `pub run build_runner watch -o js`
5. `python3 -m http.server` (in new terminal window/tab)
6. open `http://localhost:8000/js/web/some_static/index.html` in a browser and see 404 errors in the console
7. uncomment `base tag` in `index.html` to make example work, not really a solution to me...