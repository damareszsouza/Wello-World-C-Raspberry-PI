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

APÊNDICE A - MÁQUINA VIRTUAL COM RASPBERRY PI
(by Vítor Araújo Lengovski)
Além do sistema de visualização de imagens, foram realizadas outras
atividades no estágio como bolsista. Os Raspberry Pi controlam as câmeras e
disponibilizam as imagens por endereço HTTP, usando o programa Motion. Sendo
assim, fez-se necessária a criação de uma máquina virtual, usando a versão do
sistema Raspbian para computadores (Raspberry Pi Desktop). Abaixo, serão
descritas as etapas para a criação de uma máquina virtual usando VirtualBox.
Primeiramente, o usuário deve baixar o arquivo ISO, usado para gravação de
softwares e sistemas operacionais. O arquivo desse exemplo está disponível no site
do Raspberry Pi(https://www.raspberrypi.org/downloads/raspberry-pi-desktop/). Ao
entrar nessa página, clique em “Download ISO” para baixar o arquivo.
Figura 17: Baixando arquivo ISO.
Fonte: Elaborado pelo autor.
Tendo baixado o arquivo ISO do sistema, deve-se abrir o programa VirtualBox
e clicar no botão “Novo”. Após isso, nomeie a máquina virtual, selecione o tipo

“Linux” e a versão “Other Linux” e clique em “Próximo”, 

Agora escolha o quanto de memória RAM a máquina terá. O recomendado é
256 MB, mas, se possível, escolha valores maiores para um melhor desempenho.
Após escolher a quantidade, clique em “Próximo”, 
Após isso, o VirtualBox pede para configurar o disco rígido da máquina virtual.
Recomenda-se seguir a instrução padrão, selecionando “Criar um novo disco virtual
agora”. Após escolher, clique em “Criar”, 

Se o VirtualBox pedir qual tipo de arquivo de disco rígido, recomenda-se
escolher a opção padrão: “VDI (VirtualBox Disk Image)”. 
Após isso, o usuário deve escolher a forma de armazenamento no disco
rígido físico. A opção “Dinamicamente alocado” faz o espaço utilizado aumentar à
medida que se usa, enquanto que “Tamanho fixo” é criado com o tamanho máximo.
Nesse exemplo, opta-se pela segunda opção.

Por fim, o VirtualBox irá perguntar quanto espaço você deseja reservar para a
máquina virtual. Ainda que, por padrão, sejam definidos 8 GB, recomenda-se
aumentar a capacidade, se possível, para que o uso não seja limitado. Após
escolher a capacidade, clique em “Criar”.

Após criar a máquina virtual, deve-se configurá-la para a instalação do
sistema operacional. Para isso, acesse as configurações da máquina criada e entre
em “Armazenamento”. Nesta aba, selecione “Vazio”, clique no ícone de disco no
canto direito, e encontre o arquivo ISO baixado no início desta seção. Por fim clique
em “OK” para salvar as alterações.

Com o ambiente configurado, deve-se, agora, realizar a instalação do sistema
operacional. Ao iniciar a máquina, o sistema lhe dará opções de como prosseguir.

escolha “Graphical install”
e pressione Enter para começar a instalação. 

Prosseguindo com a instalação, selecione o idioma de sua preferência e
clique em “Continue”. Assim que o sistema terminar de carregar os componentesadicionais, você deverá escolher os discos de partição. Dentre as opções mostradas,
nesse exemplo, deve-se selecionar a primeira opção “Guided - use entire disk”.
Nessa opção você será questionado sobre a partição virtual em que o sistema será
instalado. Selecione a opção e clique em “Continue”, Após isso, escolha a partição virtual desejada e prossiga com a instalação. Na
próxima tela, o modo de organização de pastas deve ser escolhido, nesse caso, a
opção recomendada. Após isso, clique em “Continue”,
O sistema, agora, mostrará a visão geral de como as partições estão 
configuradas. Ainda é possível fazer alterações, mas nesse exemplo será encerrado 
o particionamento, escolhendo “Finish partitioning and write changes to disk” e 
clicando em “Continue”, Na próxima tela o sistema perguntará se o usuário deseja realizar as
mudanças no disco, selecione “Yes” e siga para a última etapa da instalação.
Nesses últimos passos, o usuário escolherá se deseja instalar o GRUB na máquina.
Esse programa possibilita escolher o sistema operacional assim que o computador
iniciar. Nesse exemplo, opta-se por instalar o programa, selecionando “Yes” e
clicando em “Continue”,

Após isso escolha em qual unidade de disco o GRUB deverá ser instalado. O
disco virtual normalmente tem seu nome iniciado por “dev/sda”. Selecione-o e
prossiga a instalação.

Assim que a instalação do GRUB terminar, o sistema informará o usuário que
a instalação está completa. Continuando, a máquina virtual terá últimos preparos e
será inicializada automaticamente. Faltam apenas configurações de hora, linguagem
e senha da máquina virtual. 

(by Vítor Araújo Lengovski)


