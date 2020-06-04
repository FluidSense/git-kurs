# Try-it-yourself!

- git checkout try-it-yourself/bisect
- With python installed:
    - Try to run `python app.py`.
    - Notice the unwanted output.
    - Take a big leap behind in the git log and checkout a commit there.
    - Try to run `python app.py` and find a commit with output that seems reasonable.
    - Mark the commit as good: `git bisect good <hash>`.
    - Mark HEAD as bad: `git bisect bad HEAD`.
    - Start the bisect: `git bisect start`.
