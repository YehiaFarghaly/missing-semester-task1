1) ```bash
     ls -alh --color=auto --time-style="+%b %d %H:%M" | sort -k6Mr -k7nr
   ```
2) ```bash
   vim marco-polo
   ```
   * press alt + i to enter the insert mode then type this [code](https://github.com/YehiaFarghaly/missing-semester-tasks/blob/main/lecture2/marco-polo.sh)  
   * press Esc button to exit insert mode, then type `:wq` to save the file <br> <br>
     
   ```bash
   source marco-polo
   marco
   cd ..
   polo
   ```
3) ```bash
    vim error-detection-script
   ```
   * press alt + i to enter the insert mode then type this [code](https://github.com/YehiaFarghaly/missing-semester-tasks/blob/main/lecture2/error-detection-script)
   * press Esc button to exit the insert mode, then type `:wq` to save the file <br> <br>
     
   ```bash
   source error-detection-script
   ```
4) ```bash
    find . -name "*.html" | xargs -d ' ' zip html_files.zip
   ```
5) ```bash
    find . -exec ls -t {} | head -n 1
   ```
