# linux-recycling-system


So... in Linux there is nothing like a recycling bin.
When you delete stuff, they are removed permenantly, unlike windows
where there's a recycling bin where you can find deleted items there until you empty
the bin.

So here is a solution, however you would need to execute the bash script to recycle stuff,
and restore stuff ofcourse.

The items will be temporarily saved in a file named bin, the abs path and it's inodes will be saved in another hidden file

Just get this script into your system, bash call it 

so command usage would be:
bash 'the script path/recycle' 'file name' -> for recycling
bash 'the script path/restore' 'file name' -> for restore !! Please beware that the file name here must be equal to the one in the .restore.info or else it would not recognize it

This also prompts the user if there is a file already under that name you would want to restore in the original location, and would ask if you would want to over-write it

This script also allows to remove all of the files sub-directories recursively using -r 

Enjoy!
