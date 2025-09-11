# linux-tips
Tips and tricks for using Linux

## Uncompress all matching files using unzstd (or whatever program is appropriate)

Use a bash for loop to get all the files. The inside the loop call the compression function.

for f in *.zst ; do unzstd "$f" ; done
