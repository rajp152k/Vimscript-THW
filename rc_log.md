## RC Log 

- a timestamped log of all the changes to my vimrc with some wisdom and insight as to why so...
- goal is to capture the evolution of my rc 
- also some things learned along the way

---
### Fri Jan 29 22:45:19 IST 2021

 - upper U , lower u in visual mode
    - `map  <c-u> vawUe`
    - handy for something like CUDA_VISIBLE_DEVICES
 - to remove a mapping, just map that key to itself
 - `map - ddp` to move a line down and `map _ ddkkp` to move a line up
 - to know what keystrokes are captured when typing a meta key: 
    - hit <c-v> in insert mode and then the key
 - included a map for logging with timestamps
    - the k and J after the return to get the date inserted on the same line
    - output from `r!` inserts an extra \n in the end
 - maps also included for editing and sourcing vimrc
 - another map for quick access to the terminal
    ```
    map <leader>l :r!date <Cr> k J
    map <leader>e :vs ~/.vimrc <Cr>
    map <leader>s :source ~/.vimrc <Cr>
    map <leader>t :ter <Cr>
    ```
 - setting line number and relative line number : 
 - line number shows the current line number as absolute and relative line number shows the others as relative : use both 
    ```
    set relativenumber
    set number
    ``` 
