# linux-tips
Tips and tricks for using Linux

## Uncompress all matching files using unzstd (or whatever program is appropriate)

Use a bash for loop to get all the files. Then inside the loop call the compression function.

> for f in *.zst ; do unzstd "$f" ; done

## Extract matching files from a tar file

Use the *--wildcards* option

> tar xf dm-100820-dmn15.tar --wildcards  "\*foobar\*"
