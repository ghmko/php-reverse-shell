# php-reverse-shell


## Stabilize reverse Shell

-Do this on Kali, zsh shell gives error with turning enter in to ^M

&emsp;&emsp;&emsp;&emsp;exec bash --login

-Check if bash is active.

&emsp;&emsp;&emsp;&emsp;ps -p $$ 

-get vars 

&emsp;&emsp;&emsp;&emsp;echo $TERM

&emsp;&emsp;&emsp;&emsp;stty -a 

-Setup shell nc 

&emsp;&emsp;&emsp;&emsp;nvlp -nc 4444

&emsp;&emsp;&emsp;&emsp;$ python -c 'import pty; pty.spawn("/bin/bash")'

&emsp;&emsp;&emsp;&emsp;Ctrl-Z

-In terminal

&emsp;&emsp;&emsp;&emsp;$ stty raw -echo

&emsp;&emsp;&emsp;&emsp;$ fg

-In reverse shell

&emsp;&emsp;&emsp;&emsp;$ reset

&emsp;&emsp;&emsp;&emsp;$ export SHELL=bash

&emsp;&emsp;&emsp;&emsp;$ export TERM=xterm-256color

&emsp;&emsp;&emsp;&emsp;$ stty rows <num> columns <cols>


-not always needed.
  
&emsp;&emsp;&emsp;&emsp;export TERM=xterm
  
  
  
  
  
  
  
  
  
  original code : https://github.com/pentestmonkey/php-reverse-shell
