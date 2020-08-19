**This is experimental and unfinished software. Use at your own risk! No warranty for any kind of damage!**

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

# Verus-Coin-Importer
A simple tool to create coin files to import into Verus Desktop.

## Usage & Installation
- To use the importer tool, you need node v12.0.0 or greater and yarn
- Currently, you can only import Komodo asset chains into Verus Desktop using this tool

1) Download this git repository to your computer
2) Using a terminal, cd into the repository
3) Run "yarn" in the terminal
4) Run "node index.js" in the terminal and answer the questions 
4) When you've filled out the form, double check that the created JSON file printed to your console is how you want it to be
5) A new file, "\<your coin ticker\>_import.txt" should be created inside the repository folder, this is your import file

## Testing your import file with Verus Desktop

1) Open Verus Desktop and navigate past the login/choose account screens to the wallet
2) Select "Add Coin" from the left side of the screen, a modal should appear with a searchable dropdown in the middle
3) Without the dropdown selected, within this modal, hit the `Alt` key three times or type "ADDFROMFILE", on your keyboard (without the quotes), the searchable dropdown should now be replaced by a file selector
4) Select "\<your coin ticker\>_import.txt" from the file selector, and press continue
5) Ensure that the buttons for the modes your coin supports arent grayed out (e.g. if your coin supports native mode, the native button is clickable)
6) Test each available mode to make sure it works, connects, can send, and gets all information properly
