### Installation

    javac -d bin main/Cal.java

### Execute it !

    java -cp bin main/Cal input.exp -o output.asm

    input.exp means the file of your logic expression

    output.asm means the file of your change result of your logic expression    

    Example:

	 input.exp:testa=2*(3*(4-5)+6)==$

	 output.asm:
	mov  eax , 4
	sub  eax , 5
	mov  ebx , 3
	mul  ebx , eax
	mov  ecx , ebx
	add  ecx , 6
	mov  edx , 2
	mul  edx , ecx
	mov  eex , 4
	sub  eex , 5
	mov  efx , 3
	mul  efx , eex
	mov  egx , efx
	add  egx , 6
	mul  edx , egx
	mov  testa , ehx
