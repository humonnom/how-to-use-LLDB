# How to use lldb?          
	Language : C           
	Tool : MAC           
---------------------------------------------------          
## 💻 lldb & gdb          
	unix 기반 시스템: gdb          
	OS X, 리눅스, 윈도우 등: lldb          
          
---------------------------------------------------          
## how to compile with lldb?         
	<gcc>       
	gcc -g [target file]          
   		ex) gcc -g test.c          
    
	<clang>       
	clang -g [target file]          
   		ex) clang -g test.c          
---------------------------------------------------          
## start lldb (2step)         
	step 1. execute lldb : lldb [exe file]          
		ex) lldb a.out          
	step 2. run lldb : just type `run`   
		ex) run   
	     	run with arguments : `r arg1 arg2`  
		ex) run a b   
		    run "a and b" "c"    
---------------------------------------------------          
## exit lldb (2methods)         
	- ^D (ctrl + d)          
    - q    
---------------------------------------------------          
## set break point & delete break point    
	<set>    
	b [file]:[line number]    
		ex) b test.c:79    
    
	<delete>    
	b delete [target/line number]    
		ex) b test.c:79    
    
	*break point = b = br    
---------------------------------------------------          
## Basic command     
	next line : n    
	quit : q    
	backtrace : bt    
	next break point : continue (or just type `c`)          
    
---------------------------------------------------          
## view frame detail    
	frame s [frame number]    
		ex) frame s 0    
		(`s` means `select`)    
    
---------------------------------------------------          
## check variable value & address    
	<value>    
	p [variable_name]    
		ex) p i    
		ex) p result    
    
	<address>    
	p &[variable_name]    
		ex) p &i    
		ex) p &result    
   
---------------------------------------------------          
##  lldb awesome    
	https://www.letmecompile.com/xcode-lldb-%EB%94%94%EB%B2%84%EA%B9%85-%ED%85%8C%ED%81%AC%EB%8B%89/    
