# github-archive-deduplicate
Get rid of duplicates that made their way into the GitHub Archive

I mostly just uploaded this so I'd have it and so that others can check my work so that GitHub events aren't lost forever.

### Scripts
* **events-per-file** to generate map of event ids to the files they are in
* **deduplicate-file** filter to remove duplicate event ids (use pipes)
* **run-deduplication** shell script to deduplicate every file containing a duplicate (from `files-containing-duplicates.txt`)

### Output
* **duplicate-event-ids.txt** duplicates that were found using above tools
* **duplicates.txt** generated from the output of `events-per-file` run through `sort` and `uniq`
* **files-containing-duplicates.txt** generated from second column of above (using `cut`)
