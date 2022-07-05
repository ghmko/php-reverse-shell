# php-reverse-shell


##################################Stabilize reverse Shell##################################
#Do this on Kali, zsh shell gives error with turning enter in to ^M
exec bash --login

# Check if bash is active.
ps -p $$ 

#get vars 
echo $TERM
stty -a 

#Setup shell nc 
nvlp -nc 4444
$ python -c 'import pty; pty.spawn("/bin/bash")'
Ctrl-Z

# In Kali
$ stty raw -echo
$ fg

# In reverse shell
$ reset
$ export SHELL=bash
$ export TERM=xterm-256color
$ stty rows <num> columns <cols>


#not always needed.
export TERM=xterm
  
  
  
  
  
  
  
  
  
  original code : https://github.com/pentestmonkey/php-reverse-shell
