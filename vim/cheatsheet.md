rayninfo.co.uk/vimtips.html

# Vim book cheatsheet - http://www.truth.sk/vim/vimbook-OPL.pdf

## Filtering, motion command

- !10GSort <Enter> <!-- From actual line to actual sort -->
- !!ls
- !!date

## Multiple Files

vim file1 file2 file3

- :wnext          <!-- write changes and go to next opened file -->
- :set autowrite  <!-- enable autowrite when you change the file -->
- :set noautowrite
- :args           <!-- display the list of the files being edited -->

## Opening a new window

- :split          <!-- split the screen into two widnwos, both editing the same file -->
- CTRL-Ww         <!-- change the selected window -->
- CTRL-Wj         <!-- change to the bottom window -->
- CTRL-Wk         <!-- change to the upper window -->

### Summary
:count split +command file

count, the size of the window in lines. Default equal size
+command, an innitial command
file, the name of the file to edit

## Changing window size

- count CTRL-W-less   <!-- decrement window size in lines by count or 1 -->
- count CTRL-W-plus   <!-- augment window size in lines by count or 1 -->
- CTRL-W-_            <!-- if no count is specified, the window is increased to its maximum size -->

## Buffers

- :hide               <!-- if there is more than one window, hide the current one -->
- :buffers            <!-- show the list of buffers -->
- :buffer number      <!-- select the buffer number -->
- :bnext              <!-- go to next buffer -->
- :sbnext             <!-- split next buffer -->

## Basic visual Mode

- v                   <!-- Enter visual mode -->
- CTRL-V              <!-- Enter visual block mode -->
- CTRL-V + I + ESC    <!-- Enter visual block mode and edit multiple lines -->
- CTRL-V >            <!-- shifts the text to the right one shift width -->
- CTRL-V <            <!-- shifts the text to the left one shift width -->

# Commands for programmers
