This is the data/ folder; a separate git repository, here: https://github.com/sutt/ppd_data .

The parent repo is https://github.com/sutt/ppd .This file should be the only thing in this folder visible to the parent repository. This git repository is separated to avoid adding binary data to the src history.

Here's how the repo is laid out:

    usr/  - use this as a local scratch folder; is gitignored

    test/ - data for tests; mostly in ppd/test/ right now

    proc/ - central folder for useful working data

        raw/ - the guirecord, isProcessed=False, vid + supplimentary files

        proc/ - processed vid + supplimentary files

    misc/ - catchall

        books/ - for data in ppd/books

        timelog_bench/ - from exploring frame timing and logging it; use this to benchmark guirecord perf (FPS) vs a previous time

