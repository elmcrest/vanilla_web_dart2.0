steps to reproduce the issue with non-relative packages

1. clone repository
2. cd into it
3. pub get
4a. pub run build_runner watch -o js
4b. python3 -m http.server (new terminal window/tab)
5. see 404 errors