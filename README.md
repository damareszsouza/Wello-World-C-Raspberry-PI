# Wello-World-C-Raspberry-PI

# Exercicio de pratica referente ao curso de Rapberry PI
Referente ao curso Raspberry PI Básico para IoT, e intenção de aprendizagem pelo site https://www.filipeflop.com/blog/linguagem-c-com-raspberry-pi/
Criação de uma máquina virtual com o Raspberry PI OS (visualização alternativa)
Apêndice do Relatório de Estágio do estudante Vítor Araújo Lengovski do curso Técnico em Informática para a Internet do campus Bento Gonçalves do IFRS.

Além do sistema de visualização de imagens, foram realizadas outras atividades no estágio como bolsista. Os Raspberry Pi controlam as câmeras e disponibilizam as imagens por endereço HTTP, usando o programa Motion. Sendo assim, fez-se necessária a criação de uma máquina virtual, usando a versão do sistema Raspbian para computadores (Raspberry Pi Desktop). Abaixo, serão descritas as etapas para a criação de uma máquina virtual usando VirtualBox.

Primeiramente, o usuário deve baixar o arquivo ISO, usado para gravação de softwares e sistemas operacionais. O arquivo desse exemplo está disponível no site do Raspberry Pi (https://www.raspberrypi.org/downloads/raspberry-pi-desktop/). Ao entrar nessa página, clique em “Download ISO” para baixar o arquivo.

#include <stdio.h>
 
int main()
{
    printf("Hello World!\n");
    return 0;
}

// Biblioteca WiringPi

//Para quem já programou Arduino vai achar bem fácil a biblioteca WiringPi. Ela foi desenvolvida para facilitar o acesso  
//controle dos pinos GPIO da Raspberry Pi. É uma biblioteca feita para uso em programas de linguagem C ou C++. Assim
//como a IDE Geany, a biblioteca WiringPi já vem instalada no sistema bastando apenas incluir a biblioteca em 
//seu programa com a linha “#include <wiringPi.h>“.
