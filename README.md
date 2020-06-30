# caixaeletronico

	funcao inicio()
	{

inteiro opcaofinal = -1

enquanto (opcaofinal != 1) menu ()


	}

	
funcao menu () {
inteiro conta, senha = 123456, opcaofinal = -1

escreva ("------- Olá cliente, seja bem vindo ao Banco do Brasil ------- \n")


escreva ("------- Digite sua conta ------- \n")
leia (conta)
enquanto (conta != 1234) {
escreva ("Por favor digite sua conta corretamente \n")
leia (conta)	
}


escreva ("------- Digite sua senha ------- \n")
leia (senha)
enquanto (senha != 123456) {
escreva ("SENHA INCORRETA, Digite sua senha \n")
leia (senha)
}

real saldo = 100.00 
real deposito, saldoAtual, saque
inteiro opcao
logico logado = verdadeiro

enquanto (opcaofinal != 2) {
escreva ("\nEscolha a opção desejada \n")
escreva ("\n1 - SAQUE \n")
escreva ("2 - REALIZAR DEPOSITO \n")
escreva ("3 - CONSULTAR O SEU SALDO \n")
leia (opcao)


escolha (opcao) {

caso 1: 
escreva ("Digite o valor que deseja sacar: \n")
leia (saque)
se (saque > 100 ) {
	escreva ("Valor indisponível, você não possui saldo suficiente \n")
} senao 
escreva ("Saque realizado com sucesso, seu saldo é:", " ", saldo - saque)
pare

caso 2:
escreva ("Digite o valor que deseja depositar na sua conta \n")
leia (deposito)
escreva ("Deposito realizado com sucesso, seu novo saldo é:", " ", saldo + deposito)
pare

caso 3: 
escreva ("Seu saldo é:", " ", saldo)
pare
}

escreva ("\nDeseja continuar logado? Digite 1 - SIM / Digite 2 - NÃO \n ")
leia (opcaofinal)
limpa ()

}

}
