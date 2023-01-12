1. Using the echo command print in console "Hello World". Here is some info about echo command [https://discuss.codecademy.com/t/what-are-practical-uses-of-the-echo-command/394788] DONE
		R:  echo "Hello World"

2. Create a new directory called `new_dir`. DONE
		R: mkdir new_dir

3. Delete/Remove the directory `new_dir`. DONE
		R: RM -rf new dir

4. Copy the file `sed.txt` from the `lorem` folder and paste it to the folder `lorem-copy` folder. DONE
		R: cd lorem
		   cp sed.txt ../
		   cd ../
		   cp sed.txt lorem-copy.txt

5. Copy the other two files from the `lorem folder` to `lorem-copy` folder in just one line using semicolon `;`. DONE
		R:
		cd lorem
		cp at.txt lorem.txt 

6. Show the `sed.txt` file content from the `lorem` folder. DONE
		R:  cd lorem
			cat at.txt lorem.txt

7. Show the `at.txt` file and `lorem.txt` file contents from `lorem` folder. DONE
		R: cat lorem/at.txt;lorem.txt

8. Print the first 3 rows in `sed.txt` file from lorem-copy folder. DONE
		R: head -3 sed.txt

9. Print the last 3 rows in `sed.txt` file from lorem-copy folder. DONE 
		R: tail -3 sed.txt

10. Add `Homo homini lupus.` at the end of `sed.txt` file in the `lorem-copy` folder. -DONE
		R: echo "Homo homini lupus" >> sed.txt

11. Print the last 3 rows in `sed.txt` file from `lorem-copy` folder. You should see `Homo homini lupus.`. DONE
		R: tail -3 sed.txt

12. `sed` command is used to replace the text in a file. Use the `sed` command to replace all occurances of `et` with `ET` in the file `at.txt` file present in the folder `lorem`. You can use the following link to refer to `sed` commands [https://www.linode.com/docs/guides/manipulate-text-from-the-command-line-with-sed/] DONE
Check the contents of the sed.txt file using `cat` command. 
		R: sed -i 's/et/ET/g' at.txt
			cat at.txt

13. Find who is the system user.  DONE
		R: whoami

14. Find the current path of the directory you are in. DONE
		R: pwd 

15. List all files with the extension `.txt` in lorem folder. DONE
		R: ls ../lorem-copy *.txt
16. Count the rows in `sed.txt` file from lorem folder. Look concatenate `cat` and `wc` with the pipe `|`. DONE
		R:  cat|wc -l sed.txt

17. Count the **files** which start with `lorem` in all directories. DONE

	R: ls -1 | grep ^"lorem" | wc -l
