# Automating GIS processes: notebooks used during the lessons at the University of Helsinki

This repository contains the notebooks used in contact-teaching. The [docker image used for CSC
Notebooks](https://github.com/Automating-GIS-processes/csc-notebook-dockerfile)
clones (or fetches and merges) this repository upon start.

To prepare these files, use `jupytext` to convert the markdown-based notebooks from
[Automating-GIS-processes/site](https://github.com/Automating-GIS-processes/site),
then remove the code from cells that should be filled during the lesson.

If you want to add the lessons one-by-one as the course proceeds (e.g., every
week), you can clone this repository locally in the beginning of the teaching
period, run `git rm --cached -r lesson-?` to remove all lessons from the index (but
keep a local copy), commit and push. Each week, you can then use `git add lesson-1`,
commit and push, to upload the new content.

**At the beginning of the teaching period**, remember to replace `environment.yml` with an
updated listing all packages pinned to the current year’s versions (see the [README in 
`Automating-GIS-processes/site`](https://github.com/Automating-GIS-processes/site/blob/main/README.md)).
