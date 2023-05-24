# Fundamentos_Robótica_Grupo_NAO_Coreograph

Repositório destinado ao trabalho da matéria de robótica da Fga. 

![kisspng-humanoid-robot-nao-robotics-robot-png-photos-5a753cb9b65847 3118324815176326977469](https://github.com/lara-unb/Fundamentos_Robotica_NAO_Coreograph/assets/89438448/158c388a-58d0-48e4-a2dc-f837e555c806)

## Descrição do Projeto (NAO - Coreograph)  

### Regras gerais:  
**1.** Serão 5 entregas semanais nas quinta-feira 23h59, a partir da semana 8 (16/05/23). Atraso acarretará em desconto de 10% por dia de atraso.  
**2.** Cada entrega será feita no GitHub e deve conter  
  **2.1.** Código tipo "demo" - só baixar e rodar  
  **2.2.** vídeo do robô executando a demo - subir no youtube e colocar o link 
  **2.3.** documentação: descrição da demo na própria página do GitHub (markdown)  
**3.** Apresentação oral no retorno do professor 

### Projeto:
**1.** Criar uma apresentação para cada entrega;  
**2.** Ao menos duas com interações com usuários via sensores do robô;

### Integrantes:
Carlos Eduardo Leite de Oliveira - 170007707 

Breno Linhares de Sousa - 170007057

Haniel Rodrigues Guimaraes de Lima – 150036558

Vitor Rangel de Aquino Silva – 170064107

# PROJETO 01 - Definindo Ações por Reconhecimento de Fala 

# Resumo

Para o primeiro projeto o grupo escolheu realizar as tarefas no Robô NAO e a programação foi realizada no softwre Coreography 2.8.6.23  disponível em: https://www.aldebaran.com/en/support/nao-6/downloads-softwares.

A primeira tarefa desenvolvida pelo grupo foi fazer o NAO ouvir e reconhecer palavras em português e realizar diferentes ações de acordo com a palavra pronuciada como *Sentar*, *Levantar*, *Falar* e *Pegar*. Especificamente na ação *Pegar* o NAO procura uma bola vermelha e anda até a bola e na ação *Falar* o NAO emita o latido de um cachorro.

## Conteúdo

- [Introdução](#1)
- [Video](#2)
- [Implementação](#3)
- [Código](#3)

<a id='1'></a>

## Instrodução

Para a implementação dessa atividade no NAO foram utilizados os microfones, alto falantes e câmera do NAO para o reconhecimento da fala, para reprodução da fala e para o processamento de imagem para detecção da bola vermelha, além de outros sensores e atuadores como motores de passo e giroscópios para o movimento das juntas do robô. A imagem abaixo detalha melhor a localização dos microfones e a câmera presente nos olhos. 

![sensores](https://github.com/themestrre/Grupo-NAO-Coreograph-/assets/89438448/39ac133a-d499-4dd6-be05-ccbe49dafa61)


<a id='2'></a>
## Vídeo

O vídeo mostrando os testes do programa implementado pelo Grupo pode ser acessado pelo seguinte link: https://www.youtube.com/watch?v=vUP44cZrWn8&ab_channel=BrenoLinhares

<a id='3'></a>
## Implementação

A figura abaixo mostra o diagrama de blocos montado no software coreography. O diagrama realiza as seguintes tarefas:

1. Reconhecer a palavra pronuciada - implementada pelo bloco *"SPEECH RECO"* ;
2. Utilizar um *swich case* para selecionar entre as palavras *"Senta"*, "*Levanta"*, *"Late"* e *"Pega"*;
3. Dependendo da palavra reconhecida o NAO realiza a respectiva ação;
4. Primeira ação *Sentar* - implementada pelo bloco "SIT DOW";
5. Segunda ação *Levantar* - Implementada pelo bloco "STAND UP";
6. Terceira ação *Latir* - Implementada pelo bloco "SAY" configurado para reproduzir o texto "AU AU AU AU";
7. Quarta ação reconhecer e caminhar até a bola - Implementada pelos blocos "RED BALL TRACKER" e "MOVE TO"

Todas as saídas dos blocos de ação são realimentados ao bloco *"SPEECH RECO"* para que o NAO possa reconhecer novas palavras após terminar de realizar a ação atual. 

![Diagrama de Blocos](https://github.com/themestrre/Grupo-NAO-Coreograph-/assets/89438448/9d785fe5-d8f0-4762-9b52-f985a150fd5c)

OBS: No bloco *"SPEECH RECO"* foi configurado um threshold de 40 como sensibilidade para reconhecimento dos padrões da fala.

<a id='4'></a>
## Código
O Código implementado pode ser acessado na pasta [Projeto_1](https://github.com/themestrre/Grupo-NAO-Coreograph-/tree/main/PROJETO_1) deste repositório. 



# PROJETO 02 - 

# PROJETO 03 - 

# PROJETO 04 - 

# PROJETO 05 - 
