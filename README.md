# About
This tool is intended for use in the Nation Song Contest, an online forum-based music sharing game with a format based on the Eurovision Song Contest. The tool generates banners using ASCII art, based on ASCII flags placed in the `Flags-ASCII` folder and entry data entered in the spreadsheet `entries.xlsx`.

# Requirements
This tool uses the third party module OpenPyXL. Please install this module before attempting to run the Python scripts included here.

# Instructions
1. Enter the nation names, artist names, song titles, and (optionally) URLs in the corresponding columns in the spreadsheet `entries.xlsx`.
2. Convert the nations' flags to ASCII art using `https://www.ascii-art-generator.org/`, using a width of 60 characters. Download the resulting .txt files and save them to the `Flags-ASCII` folder. Name the .txt files according to the nation names listed in `entries.xlsx`. You may alternatively create your own ASCII art for each nation.
3. Run `banner_generator.py`. This will generate ASCII banners using the data in `entries.xlsx` together with the ASCII flags in the `Flags-ASCII` folder, saving them to the `Banners` folder.
4. (Optional) Run `show_generator.py`. This will create the file `show.txt`, which contains all the banners with URLs added (ordered according to `entries.xlsx`), written in BBCode so that it can be pasted into a forum post. Please note, this may need to be split into several posts, due to the forum's character limit.