# intro-st
Introdução à programação na linguagem ST, na matéria de automação, parte do componente curricular do curso técnico de eletrônica na Fundação Escola Técnica Liberato Salzano Vieira da Cunha.

## Propostas:
*as transcrições abaixo foram feitas por Lucas Mallmann no [seu próprio repositório de programação na linguagem ST](https://github.com/LucasMallmannEich/Simple_ST_Projects)

Exercício 1:
- Três cargas devem ser acionadas em sequência, comandadas por um único botão.
- A cada toque no botão, uma das cargas é acionada.
- Um segundo botão realiza o desligamento das cargas.
- Elabore um programa que realize este acionamento.
- Utilize o Function Block R_TRIG para a detecção de borda do botão.

Exercício 2:
- Elabore um acionamento sequencial de três cargas usando um botão.
- A segunda carga aciona 5s após a primeira carga ser acionada, e a terceira 5s após a segunda.
- Implementar um botão de desligamento das cargas Utilize o Function Block TON para temporização.

Exercício 3:
- A lixa de uma lixadeira de fios deve ser afiada periodicamente, e para isto o sentido de rotação do motor deve ser invertido.
- Para isto, o controle possui duas saídas digitais, uma que aciona a o motor no sentido de lixamento, outra que aciona o motor no sentido de afiação.
- O painel de operação possui um botão de partida e um botão de parada apenas para operação de lixamento, e o painel de manutenção possui um botão de afia e um de parada de emergência que atua nos dois modos (lixamento e afiação - todos são entradas digitais do CP).
- O eixo da máquina possui um sensor de rotação (uma entrada digital do CP, será simulada manualmente), que indica se o eixo está girando (#1) ou parado (#0).
- A lógica de acionamento dita que o motor só pode ser acionado quando seu eixo estiver parado.
- Caso seja comandado para trocar de direção com o eixo em movimento, o comando deve efetuar o desligamento do movimento e aguardar novo comando somente quando o eixo estiver parado.
- Elabore um programa que implemente esta lógica.
- No display da IHM devem ser exibidos o status do motor (‘OPERAÇÃO’ ou ‘AFIAÇÃO’), do sensor de rotação (‘MOTOR GIRANDO’ ou ‘MOTOR PARADO’).

Exercício 4:
- Elabore um comando liga-desliga para uma bomba de enchimento de um reservatório utilizando um sensor de nível (0,00V a 10,00V) em uma entrada analógica.
- Acione a bomba (saída digital) quando a tensão de entrada for igual ou inferior a 30% do valor máximo da entrada e desligue a bomba quando a tensão de entrada for igual ou superior a 70% do valor máximo.
- A IHM deve exibir as mensagens ‘NIVEL BAIXO’, ‘NIVEL NORMAL’ E ‘NIVEL ALTO’ DE ACORDO com os o valor do sensor comparado com os limiares percentuais.
- Caso um botão do painel (entrada digital), denominado emergência, seja acionado, a carga deve ser desligada e não pode ser acionada por um período de 5 segundos.
- O valor máximo deve ser editado pela IHM (entrada de texto), e salvo em uma variável de programa não volátil através de um botão da IHM.
- O valor de tensão da medição de nível, e do valor máximo também devem ser exibidos no display da IHM.

Exercício 5:
- A iluminação de uma sala é comandada em 3 pontos diferentes, através de interruptores.
- Desenvolva um programa que, a cada alteração do estado de um dos interruptores, troque o estado da lâmpada, ou seja, cada vez que um dos interruptores é ligado ou desligado, a lâmpada acende se estava apagada, ou apaga se estava acesa.

Exercício 6:
- A saída de veículos normalmente é sinalizada por duas lâmpadas, que piscam alternadamente.
- Elabore um programa que realize esta função, a partir da ativação de um sensor de porta de garagem aberta (entrada digital, #0: porta fechada, #1: porta aberta).
- Ao ser fechada a porta, as lâmpadas permanecem piscando por 5 segundos.
- Utilize uma frequência de piscada de 2 HZ.

Exercício 7:
- Faça um programa para inverter uma string dada (armazenar em outra variável, a variável original deve permanecer inalterada).
- Observação: a string deve poder ser modificada, em modo de execução, como sendo uma variável do programa.
- Utilizar a IHM “virtual” no computador, com uma tecla de função para realizar a inversão da string.
- Para identificar o tamanho variável, use a função LEN.
- Explore as funções orientadas a strings no help do Mastertool IEC.
- Execute e apresente apenas em modo de simulação no Mastertool IEC. VAR NOME: STRING := ‘Atropelando 2023’; TAMANHO: INT:=0; NOMEREV: STRING; ... END_VAR

