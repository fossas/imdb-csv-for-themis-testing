# large CSV file for Themis performance testing

This repo is used in Themis performance tests.

This is a subset of a large set of data used for AI training. The original file has around 50k rows in it, but that takes very long to scan with Themis if you actually read and scan the full file (I gave up after 20 minutes).

On a macbook M1 pro, this subset takes around 5 minutes to read if you actually scan the full file. But after https://github.com/fossas/themis/pull/77, we no longer read the full file and the scan should complete in < 30 seconds.
