; Exercícios conforme problemas

; DOCTYPE assembly
; assembly lang="eng" 

; Programe para somar o conteúdo do acumulador (A) com o conteúdoo de R2. Depois somar o resultado da 1a soma com o valor que estava inicialmente em A. Colocar o resultado em R7. (Na linguagem Assembly do 8051).

; Inicialmente: A=5/R2=7/R6=0/R7=0.

mov R6, A
add A, R2
add A, R6
mov R7, A
end

; Programa em assembly do 8051 pra somar 5 com o conteúdo de RØ e colocar o resultado no port PØ.

mov A, #05H
add A, RØ
mov PØ, A
end

; Programa para subtrair 100 de R4, depois somar o resultado com 20 e com o valor de P2. O resultado final deve ser escrito no registrador 2ØH.

mov A, R4
sbb A, #64H
add A, P2
mov 20H, A
end

; Programa para, se o valor no port 1 for par , divide por 2 e coloca o resultado em 3ØH, caso contrário subtrai 3 e guarda o resultado no registrador 31H.

mov A, P1
mov B, #02H
div A, B
mov A, B
JZ epar
mov A, P1
sbb A, #03H
mov 31H, A
jmp fim
epar: mov A, P1
mov B, #02H
div A, B
mov 30H, A
fim: end

; Programa: Se o n⁰ no port 2 for 15d, somar o valor do port 1 com o valor e R7, caso contrário, subtrair 1 do valor do port 1. O resultado em qualquer caso, deve ser armazenado em 20H.

mov A, P2
cjne A, #OFH, not
mov A, P1
add A, R7
jmp fim
not: mov A, P1
sbb A, #01H
fim: mov 20H, A
end
