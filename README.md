# natas13solution
This is the python script with make the php payload to bypass the exif_imagetype function of php used in natas13 (overthewire.org) challenge.

During my practice period i come into idea that the function used in the natas13 php sourcecode to detect only the image file can only be uploaded.

This is clearly written on the official php documentation(https://www.php.net/manual/en/function.exif-imagetype.php) of the exif_imagettype(), only read the first byte of the magical header or signature present in file during upload. if the magical headers found to be equal to the image type hex code ,then this file is image otherwise the exception error occur. 

list of the magic headers(in hex) for different file given at https://en.wikipedia.org/wiki/List_of_file_signatures

Then, I make the python script to write the magical header in any php payload where i.e
magical_header(atfirst must)+<?php code to execute.?>
\xFF\xD8\xFF\xEE + php code retrieve next level password(natas14).


Thank you for using this script.
                   for any query contact at insta    krn_bhargav
                                         at emailid  kkbhargavmail@gmail.com                              


