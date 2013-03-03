ilangowska@p137-05:~$ ls~/.ssh/
bash: ls~/.ssh/: Nie ma takiego pliku ani katalogu
ilangowska@p137-05:~$ 
ilangowska@p137-05:~$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/home/studpoz/ilangowska/.ssh/id_rsa): 
Created directory '/home/studpoz/ilangowska/.ssh'.
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/studpoz/ilangowska/.ssh/id_rsa.
Your public key has been saved in /home/studpoz/ilangowska/.ssh/id_rsa.pub.
The key fingerprint is:
9f:22:9a:7e:1c:c7:71:b5:3a:75:cd:f2:e7:62:84:a5 ilangowska@p137-05
The key's randomart image is:
+--[ RSA 2048]----+
|                 |
|            .    |
|           . . o |
|        . . o + o|
|       .So o = o |
|      . o.o.E . o|
|     ..o. o. . ..|
|     oo. .    o .|
|   .+.       . . |
+-----------------+
ilangowska@p137-05:~$ 
ilangowska@p137-05:~$ cat~/.ssh/id_pub
bash: cat~/.ssh/id_pub: Nie ma takiego pliku ani katalogu
ilangowska@p137-05:~$  cat~/.ssh/id_pub
bash: cat~/.ssh/id_pub: Nie ma takiego pliku ani katalogu
ilangowska@p137-05:~$  cat ~/.ssh/id_pub
cat: /home/studpoz/ilangowska/.ssh/id_pub: Nie ma takiego pliku ani katalogu
ilangowska@p137-05:~$ ls ~/.ssh/
id_rsa  id_rsa.pub
ilangowska@p137-05:~$  cat ~/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCyHxnAzihtQdhcg9j8ISh4S/IfEWcX+pbjwpq1RAQQtRPlvb8UUrH+JEVJYAWGUyShIkK1YZSSQijP/sfdfrNZJgERKzn0lo1DxR5DSkCl+vzb2jgJL0Gvijc7a4nrHU0S0qruKiC1IKY31me794ZqhtAWFycduXFpvYr2a+KeaGfC0YxZrtgmOqDBi07AOd9weJvhF9h8+zVX5kTfZO2plxZ3hBNil6N+OJ3aauURorwkQOgyqdbBgqUwprMyoBODRvX7vf0AluNCPifNX0X0T2cFcExiGpOrxxJlTayQUbw7fho0pao3o4KNqCZEGEphLYP+3Nskztg+qav50idx ilangowska@p137-05
ilangowska@p137-05:~$ git rmJP.MD
git: 'rmJP.MD' is not a git command. See 'git --help'.
ilangowska@p137-05:~$ git rm JP.MD
fatal: Not a git repository (or any parent up to mount parent /home/studpoz)
Stopping at filesystem boundary (GIT_DISCOVERY_ACROSS_FILESYSTEM not set).
ilangowska@p137-05:~$ 
ilangowska@p137-05:~$ L ~/.ssh/
L: command not found
ilangowska@p137-05:~$ ls
Dokumenty  etc	mail  Muzyka  Obrazy  Pobrane  Publiczny  Pulpit  Szablony  tmp  Wideo
ilangowska@p137-05:~$ git clone git@github.com:ilangowska/ti.git
Cloning into 'ti'...
The authenticity of host 'github.com (207.97.227.239)' can't be established.
RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
Are you sure you want to continue connecting (yes/no)? 
Host key verification failed.
fatal: The remote end hung up unexpectedly
ilangowska@p137-05:~$ git clone git@github.com:ilangowska/ti.git
Cloning into 'ti'...
The authenticity of host 'github.com (207.97.227.239)' can't be established.
RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
Are you sure you want to continue connecting (yes/no)? t
Please type 'yes' or 'no': yes
Warning: Permanently added 'github.com,207.97.227.239' (RSA) to the list of known hosts.
remote: Counting objects: 44, done.
remote: Compressing objects: 100% (38/38), done.
remote: Total 44 (delta 8), reused 0 (delta 0)
Receiving objects: 100% (44/44), 7.34 KiB, done.
Resolving deltas: 100% (8/8), done.
ilangowska@p137-05:~$ ls
Dokumenty  etc	mail  Muzyka  Obrazy  Pobrane  Publiczny  Pulpit  Szablony  ti	tmp  Wideo
ilangowska@p137-05:~$ cd ti
ilangowska@p137-05:~/ti$ ls
jp.md  JP.MD  README.md
ilangowska@p137-05:~/ti$ ls -l
razem 16
-rw-r--r-- 1 ilangowska studpoz 4955 mar  3 09:57 jp.md
-rw-r--r-- 1 ilangowska studpoz   13 mar  3 09:57 JP.MD
-rw-r--r-- 1 ilangowska studpoz  748 mar  3 09:57 README.md
ilangowska@p137-05:~/ti$ git rm JP.MD
rm 'JP.MD'
ilangowska@p137-05:~/ti$ git status
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	deleted:    JP.MD
#
ilangowska@p137-05:~/ti$ git commit -m "usunieto plik"
[master 8763867] usunieto plik
 Committer: Iwona Łangowska <ilangowska@p137-05.labpk.inf.ug.edu.pl>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly:

    git config --global user.name "Your Name"
    git config --global user.email you@example.com

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 deletion(-)
 delete mode 100644 JP.MD
ilangowska@p137-05:~/ti$ git config --global user.name "Iwona Langowska"
ilangowska@p137-05:~/ti$  git config --global user.email zifi@vp.pl
ilangowska@p137-05:~/ti$ git status
# On branch master
# Your branch is ahead of 'origin/master' by 1 commit.
#
nothing to commit (working directory clean)
ilangowska@p137-05:~/ti$ git push
Counting objects: 3, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 282 bytes, done.
Total 2 (delta 0), reused 0 (delta 0)
To git@github.com:ilangowska/ti.git
   c024519..8763867  master -> master
ilangowska@p137-05:~/ti$ git status
# On branch master
nothing to commit (working directory clean)
ilangowska@p137-05:~/ti$ git status
# On branch master
nothing to commit (working directory clean)
ilangowska@p137-05:~/ti$ git status
# On branch master
nothing to commit (working directory clean)
ilangowska@p137-05:~/ti$ cdDuwnloads/
bash: cdDuwnloads/: Nie ma takiego pliku ani katalogu
ilangowska@p137-05:~/ti$ ls
jp.md  README.md
ilangowska@p137-05:~/ti$ cd
ilangowska@p137-05:~$ ls
Dokumenty  etc	mail  Muzyka  Obrazy  Pobrane  Publiczny  Pulpit  Szablony  ti	tmp  Wideo
ilangowska@p137-05:~$ cd Pobrane
ilangowska@p137-05:~/Pobrane$ ls
Sublime Text 2.0.1.tar.bz2
ilangowska@p137-05:~/Pobrane$ ls -l
razem 5472
-rw-r--r-- 1 ilangowska studpoz 5587508 mar  3 10:59 Sublime Text 2.0.1.tar.bz2
ilangowska@p137-05:~/Pobrane$ tar jxvf
tar: Stara opcja `f' wymaga argumentu.
Użyj `tar --help' albo `tar --usage' żeby otrzymać więcej informacji
ilangowska@p137-05:~/Pobrane$ tar jxvf S
tar (child): S: Nie można open: Nie ma takiego pliku ani katalogu
tar (child): Error is not recoverable: exiting now
tar: Child returned status 2
tar: Error is not recoverable: exiting now
ilangowska@p137-05:~/Pobrane$ tar jxvf Sublime\ Text\ 2.0.1.tar.bz2 
Sublime Text 2/
Sublime Text 2/Pristine Packages/
Sublime Text 2/Pristine Packages/Lisp.sublime-package
Sublime Text 2/Pristine Packages/TCL.sublime-package
Sublime Text 2/Pristine Packages/Text.sublime-package
Sublime Text 2/Pristine Packages/Default.sublime-package
Sublime Text 2/Pristine Packages/Java.sublime-package
Sublime Text 2/Pristine Packages/Graphviz.sublime-package
Sublime Text 2/Pristine Packages/User.sublime-package
Sublime Text 2/Pristine Packages/Ruby.sublime-package
Sublime Text 2/Pristine Packages/CSS.sublime-package
Sublime Text 2/Pristine Packages/Groovy.sublime-package
Sublime Text 2/Pristine Packages/SQL.sublime-package
Sublime Text 2/Pristine Packages/Erlang.sublime-package
Sublime Text 2/Pristine Packages/C++.sublime-package
Sublime Text 2/Pristine Packages/D.sublime-package
Sublime Text 2/Pristine Packages/AppleScript.sublime-package
Sublime Text 2/Pristine Packages/Batch File.sublime-package
Sublime Text 2/Pristine Packages/Theme - Default.sublime-package
Sublime Text 2/Pristine Packages/OCaml.sublime-package
Sublime Text 2/Pristine Packages/ASP.sublime-package
Sublime Text 2/Pristine Packages/XML.sublime-package
Sublime Text 2/Pristine Packages/Scala.sublime-package
Sublime Text 2/Pristine Packages/Textile.sublime-package
Sublime Text 2/Pristine Packages/ActionScript.sublime-package
Sublime Text 2/Pristine Packages/Language - English.sublime-package
Sublime Text 2/Pristine Packages/Lua.sublime-package
Sublime Text 2/Pristine Packages/Go.sublime-package
Sublime Text 2/Pristine Packages/RestructuredText.sublime-package
Sublime Text 2/Pristine Packages/C#.sublime-package
Sublime Text 2/Pristine Packages/Perl.sublime-package
Sublime Text 2/Pristine Packages/Markdown.sublime-package
Sublime Text 2/Pristine Packages/Vintage.sublime-package
Sublime Text 2/Pristine Packages/Color Scheme - Default.sublime-package
Sublime Text 2/Pristine Packages/Python.sublime-package
Sublime Text 2/Pristine Packages/Objective-C.sublime-package
Sublime Text 2/Pristine Packages/R.sublime-package
Sublime Text 2/Pristine Packages/Matlab.sublime-package
Sublime Text 2/Pristine Packages/Diff.sublime-package
Sublime Text 2/Pristine Packages/JavaScript.sublime-package
Sublime Text 2/Pristine Packages/ShellScript.sublime-package
Sublime Text 2/Pristine Packages/Regular Expressions.sublime-package
Sublime Text 2/Pristine Packages/LaTeX.sublime-package
Sublime Text 2/Pristine Packages/Haskell.sublime-package
Sublime Text 2/Pristine Packages/Clojure.sublime-package
Sublime Text 2/Pristine Packages/HTML.sublime-package
Sublime Text 2/Pristine Packages/Makefile.sublime-package
Sublime Text 2/Pristine Packages/Rails.sublime-package
Sublime Text 2/Pristine Packages/PHP.sublime-package
Sublime Text 2/Pristine Packages/YAML.sublime-package
Sublime Text 2/Icon/
Sublime Text 2/Icon/16x16/
Sublime Text 2/Icon/16x16/sublime_text.png
Sublime Text 2/Icon/128x128/
Sublime Text 2/Icon/128x128/sublime_text.png
Sublime Text 2/Icon/32x32/
Sublime Text 2/Icon/32x32/sublime_text.png
Sublime Text 2/Icon/48x48/
Sublime Text 2/Icon/48x48/sublime_text.png
Sublime Text 2/Icon/256x256/
Sublime Text 2/Icon/256x256/sublime_text.png
Sublime Text 2/lib/
Sublime Text 2/lib/python26.zip
Sublime Text 2/sublime_plugin.py
Sublime Text 2/sublime_text
Sublime Text 2/PackageSetup.py
ilangowska@p137-05:~/Pobrane$ tar jxvf Sublime\ Text\ 2.0.1.tar.bz2 CD
tar: CD: Nie znalazłem w archiwum
tar: Zakończenie w stanie błędu z powodu uprzednich błędów
ilangowska@p137-05:~/Pobrane$ tar jxvf Sublime\ Text\ 2.0.1.tar.bz2 cd
tar: cd: Nie znalazłem w archiwum
tar: Zakończenie w stanie błędu z powodu uprzednich błędów
ilangowska@p137-05:~/Pobrane$ cdS
No command 'cdS' found, did you mean:
 Command 'cdb' from package 'tinycdb' (main)
 Command 'cdo' from package 'cdo' (universe)
 Command 'cdi' from package 'cdo' (universe)
 Command 'cdv' from package 'codeville' (universe)
 Command 'cdw' from package 'cdw' (universe)
 Command 'cdp' from package 'irpas' (multiverse)
 Command 'cd5' from package 'cd5' (universe)
cdS: command not found
ilangowska@p137-05:~/Pobrane$ cd Sublime\ Text\ 2
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ 
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ cd Sublime\ Text\ 2
bash: cd: Sublime Text 2: Nie ma takiego pliku ani katalogu
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ cd S
bash: cd: S: Nie ma takiego pliku ani katalogu
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ls -l
razem 7820
drwxrwxr-x 7 ilangowska studpoz       0 lip 14  2012 Icon
drwxrwxr-x 2 ilangowska studpoz       0 lip 14  2012 lib
-rw-r--r-- 1 ilangowska studpoz    4205 lip 14  2012 PackageSetup.py
drwxrwxr-x 2 ilangowska studpoz       0 lip 14  2012 Pristine Packages
-rw-r--r-- 1 ilangowska studpoz   10838 lip 14  2012 sublime_plugin.py
-rw-r--r-- 1 ilangowska studpoz 7972576 lip 14  2012 sublime_text
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ chmod  755 sublime_text 
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ls -l
razem 7820
drwxrwxr-x 7 ilangowska studpoz       0 lip 14  2012 Icon
drwxrwxr-x 2 ilangowska studpoz       0 lip 14  2012 lib
-rw-r--r-- 1 ilangowska studpoz    4205 lip 14  2012 PackageSetup.py
drwxrwxr-x 2 ilangowska studpoz       0 lip 14  2012 Pristine Packages
-rw-r--r-- 1 ilangowska studpoz   10838 lip 14  2012 sublime_plugin.py
-rwxr-xr-x 1 ilangowska studpoz 7972576 lip 14  2012 sublime_text
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ./sublime_text
            
^C              
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ./sublime_text
^[[A^C
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ./sublime_text
^[[^C
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ./sublime_text
^C
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ^Csublime_text
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ^C
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ^C
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ^C
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ ^C
ilangowska@p137-05:~/Pobrane/Sublime Text 2$ 
