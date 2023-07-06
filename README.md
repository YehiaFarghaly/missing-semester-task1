# missing-semester-task1

## Steps:

1) ```bash
    echo $SHELL
   ```
2) ```bash
   mkdir -p tmp/missing
   ```  
3) ```bash
     cd tmp/missing
     touch semester.sh
      ```  
4)    ```bash
         echo "#\!/bin/sh" > semester.sh
         echo "curl --head --silent https://missing.csail.mit.edu" >> semester.sh
         ./semester.sh
      ```  
<hr>
 <b>Notes</b>
 <br>
 1) The script does not work because the owner does not have an excute permission.
 <br>
 <br>
 2) While using `sh` command reads and excutes the script from the file directly without needing any permission so it works fine.
 <br>
 <br>
 3) the shell infers that the file should be interpreted using the sh command based on the <b><i>shebang</i></b> line <b>(#!/bin/sh)</b> present at the beginning of the semester.sh script.
<hr>

5) ```bash
   chmod +x semester.sh
   ```
6) ```bash
    ./semester.sh | grep "last-modified" | cut -d ' ' -f 2- >last-modified.txt
   ```

   <hr>
   <b> Note that: </b> <br>
   `grep` command picks the lines that contains "last-modified" <br>
   `cut` command picks the text after the second space
   <hr>
7) ```bash
   cat /sys/class/power_supply/battery/capacity 
   ```
   
