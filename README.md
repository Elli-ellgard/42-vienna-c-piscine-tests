# 42-vienna-c-piscine-tests
Testing Tools For The 42 Vienna Piscine

# What setup_project.sh does
1. Create all the required directories and files of a project

# What the tests do
1. Call the functions with some test data
2. Execute norminette
3. List all the Files that git will push to your repo (so you can make sure that the test files will not be in your final repo)

# Usage:
1. Move main.c, test.sh and setup_project.sh to the root of your project repo
2. Create all the exercise directories and required files for the project with `bash setup_project.sh n` (where n is the C Project number, e.g. if you are working on c01 enter `bash setup_project.sh 1`
3. Comment out the tests that you don't want to execute in the main.c file in int main()
4. Execute test.sh with `bash test.sh` (or `chmod 755 test.sh` first to execute with `./test.sh`)
5. Add main.c and test.sh to .gitignore (if they weren't already added by step 1)

# Known Issues:
- c01: Only checks for c01/ex00-ex07 (didn't do ex08)
- c02: Only checks for c02/ex00-ex10 (didn't do ex11 and ex12)
- Throws an error if you declare a function twice, like ft_swap() in one file and in another. For Moulinette this shouldn't be a problem but the testing script has a problem with that. Workaround: Rename the second function, i.e. to ft_swap2()
- setup_project.sh: Doesn't create correctly create files if an exercise requires more than one file

# Feedback
Feel free to use the tests and scripts, feedback and modify them. If you have any questions or want to help, write me on Discord: Francis Rafal#1334
