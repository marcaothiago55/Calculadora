# Calculadora
Este código é um projeto de uma calculadora desenvolvido pelo Professor Thiago. Ele utiliza a biblioteca U8g2 para controlar um display OLED com o controlador SSD1306. Além disso, o projeto inclui um teclado matricial com 16 botões (organizados em uma matriz 4x4) para entrada de dados.
Display OLED (SSD1306):

Controlador: SSD1306
Biblioteca Utilizada: U8g2lib.h
Inicialização: U8G2_SSD1306_128X64_NONAME_F_SW_I2C
Conexão: Utiliza os pinos SCL (clock), SDA (dados), e nenhum pino de reset específico.
Teclado Matricial:

Configuração: Matriz 4x4
Botões:
Números de 0 a 9
Operadores Matemáticos: +, -, *, /
Botões Especiais: C (limpar), = (calcular)
Pinos de Controle do Teclado:

Pinos Configurados como Entrada: 2, 3, 4, 5
Pinos Configurados como Saída (para colunas): 6, 7, 8, 9
Uso de Pull-up: INPUT_PULLUP
Buffer de Entrada:

Nome: inputBuffer
Tamanho: 16 caracteres
Uso: Armazena a expressão inserida pelo usuário.
Variáveis de Controle:

bufferIndex: Índice atual no buffer de entrada.
displayResult: Indica se o resultado deve ser exibido.
Resultado do Cálculo:

Variável: result
Tipo: Float
Utilizado para armazenar o resultado do cálculo da expressão.
Configuração Inicial no Setup():

Inicialização do Display e Configuração da Fonte.
Configuração dos Pinos de Controle do Teclado.
Limpeza do Buffer de Entrada.
Loop Principal (loop()):

Leitura do Teclado e Atualização do Buffer de Entrada.
Avaliação da Expressão e Exibição do Resultado no Display.
Tratamento de Comandos Especiais (Limpar, Calcular).
Atualização Contínua do Display OLED.
Esse projeto é uma calculadora interativa que utiliza um display OLED para exibir expressões matemáticas inseridas por meio de um teclado matricial. Os resultados dos cálculos são mostrados no display, proporcionando uma interface simples para operações matemáticas básicas.
