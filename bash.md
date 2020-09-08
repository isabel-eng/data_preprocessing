# Bash examples

*
``` mkdir data_preprocessing``` : creates a new directory name 'data_preprocessing'.

```cd data_preprocessing``` : change directory to'data_preprocessing.

``` history``` : shows all the commands used so far.

```clear``` : erases the screen.

```ls``` : shows the content of the current directory.

```nano filetext.txt``` : opens a text editor named filetext.txt .

```cat ``` : shows the content of the file.

```cp filetext.txt fileout.txt``` : copy the cotent in filetext to new fileout.

```cp -i *.txt``` copy all files that end in .txt .

```cp -R my_dir2 my_dir3```: copy content of dir 2 to dir3.

```pwd``` : show the directory where you are working.

 ```rm   fileout.txt``` : removes a single file.

 ```rm *.txt``` : removes all .txt files

 ```ls .*``` : shows the hidden files. 

```nano .file.txt``` creates a hidden file name file.txt

```rmdir my_dir``` removes the directory

```mv filetext myfile.out``` changes the name of the filetext.txt to myfile.out

```cp * ../my_dir/.``` : copy all files to my_dir

```mv myfile.out ../.``` moves myfile.out to the previous directory

```ls -l``` shows the content as a list

```ls -a``` shows ALL the content, even hidden files.

```find ./my_dir -name myfile.out``` : search the file myfile.out in the my_dir directory.

```find ./my_dir -name *.txt*``` : gives all files that end with .txt .

```find ./my_dir -empty``` : finds all empty directories or sub-directories.

```find ./ -type -name "*.txt" -exec grep 'Hello' {} \ ``` : prints the lines with the word hello in them. 'type f' specifies the input type is a file.