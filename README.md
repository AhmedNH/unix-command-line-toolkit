# Hands-On Practice with Unix Utilities and Shell Functionalities

A documented walkthrough of 89 Unix shell exercises covering file management, text processing, regular expressions, permissions, sorting, and shell quoting — all run on a live Linux system.

---

## Topics Covered

### File and Directory Management
Creating, copying, moving, and removing files and directories using `cp`, `mv`, `rm`, `mkdir`, `rmdir`, `find`, and `ls` with various flags (`-l`, `-R`, `-lt`, `-lS`, `-ltr`, `-lSr`).

```bash
cp /path/to/file .            # copy into current directory
mv xFile1 xFile2 dir/         # move multiple files at once
rm -rf lab6a                  # force-remove a non-empty directory
find . -name "xFile*" -exec chmod 775 {} \;   # find + execute on results
```

### Permissions and `chmod`
Modifying file permissions using both symbolic and octal notation, and observing the effect on file access.

```bash
chmod u-r xFile1      # remove read from owner
chmod 775 xFile1      # set rwxrwxr-x
chmod g-w,o+rw xFile1 # compound symbolic change
```

### Text Processing
Reading, concatenating, and processing file content with `cat`, `more`, `head`, `tail`, `wc`, `sort`, `uniq`, `cut`, `cmp`, and `diff`.

```bash
cat xFile1 xFile2 xFile3 > xFile123        # concatenate into one file
sort xFile123 | uniq > xFile123compact      # sort and deduplicate
sort -k6,6nr xFile123compact                # sort by field 6, numeric, reverse
cut -f 1,3 22Fclasslist                     # extract fields 1 and 3
diff xFile2 xFile3                          # show line differences
```

### Regular Expressions with `egrep`
Pattern matching across files using basic patterns, word boundaries, anchors, character classes, and alternation.

```bash
egrep ' 2 ' xFile123compact          # exact match with spaces
egrep '195.' xFile123compact         # any character wildcard
egrep '\bLi\b' 22Fclasslist         # whole-word match
egrep '\b(Liu|Lau)\b' 22Fclasslist  # alternation
egrep '^sea' lyrics                  # line anchor
egrep '1980$' lyrics                 # end-of-line anchor
egrep '[0-9]' lyrics                 # character class
egrep -v '\bthe\b' lyrics            # invert match
```

### Shell Features
Variable assignment, command substitution, quoting rules, exit codes (`$?`), and logical operators (`&&`, `||`).

```bash
echo "There are $(wc -l < 22Fclasslist) students"   # command substitution
courseN=EECS2031; echo "course is $courseN"           # variable expansion
egrep -w Zhu 22Fclasslist && echo HELLO               # short-circuit AND
egrep -w Choi 22Fclasslist || echo HELLO              # short-circuit OR
echo $?                                                # check exit code
```

### Glob Patterns
Matching files using `?`, `*`, `[...]`, and `[a-z]` wildcard patterns in `ls` and `wc`.

```bash
ls xFile?.Lab6        # single-character wildcard
ls xFile[1,3].Lab6    # character set
ls xFile[1-3].Lab6    # character range
wc -l xFile*.Lab6     # count lines across all matches
```

---

## Project Structure

```
Hands-On Practice with Unix Utilities and Shell Functionalities/
└── Project.txt    # All 89 exercises with commands and their exact output
```
