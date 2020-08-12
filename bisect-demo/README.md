# Try-it-yourself!

- `git checkout try-it-yourself/bisect`
- With python installed:
    - Try to run `python app.py`.
    - Notice the unwanted output.
    - Take a big leap behind in the git log and checkout a commit there.
    - Try to run `python app.py` and find a commit with output that seems reasonable.
    - Start the bisect: `git bisect start`.
    - Mark the commit as good: `git bisect good <hash>`.
    - Mark HEAD as bad: `git bisect bad HEAD`.
    - Run `python app.py` in the commit you are moved to.
    - If reasonable output, mark as good.
    - If not, mark as bad.
    - Repeat until bisect says 0 more commits
        - This can be seen by trying `git bisect next` which will take you nowhere
