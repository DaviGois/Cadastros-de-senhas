# Cadastros-de-senhas
Fonte para cadastrar senhas
#include <stdio.h>
#include <stdlib.h>
#include <conio.h>
#include <ctype.h>
int main (void){
int sair = 0;
char op;
int NovaSenha;
int SubsSenha;
int OldSenha;
while(sair == 0)
{
system("cls");
printf("\tMENU:\n");
printf("1 - Cadastrar uma nova senha\n");
printf("2 - Alterar senha \n");
printf("3 - Consultar senha\n");
printf("S - Sair\n");
printf("\nEscolha a opcao: ");
scanf("%s",&op);
switch(op) {
case '1':
printf("\n Insira a nova senha\n");
scanf("%d", &NovaSenha);
if (NovaSenha == SubsSenha){
printf("\n Senha já cadastrada\n");
}
getch();
break;
case '2':
printf("\n Digite senha atual:\n");
scanf("%d", &OldSenha);
if (OldSenha == NovaSenha){
printf("\n Digite a nova senha:\n");
scanf("%d", &SubsSenha);
}
printf("\n Senha alterada com Sucesso!\n");
getch();
break;
//fflush(stdin);
case '3':
printf('Sua senha e:\n");
printf(NovaSenha);
getch();
break;
case 's': case 'S':
printf("\n Saindo... TECLE ENTER!\n\n");
getch();
sair = 1;
break;
default:
printf("\nInvalido!\n\n");
getch();
break;
} }
}
