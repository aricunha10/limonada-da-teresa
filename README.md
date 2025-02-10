# 🍋 Jogo da Limonada da Teresa  
Um jogo simples feito em C, onde joga na pele da Teresa, que tem a sua própria banca de limonada!  

## 📌 Sobre o Projeto  
O **Jogo da Limonada** é um simulador onde o jogador deve tomar decisões estratégicas para maximizar o lucro da banca de limonada. O jogo envolve fatores como preços, stock e até mesmo a meteorologia! 🌦️  

## 🎮 Como Jogar  
1. **Defina o preço da limonada** com base no custo dos ingredientes e na procura dos clientes.  
2. **Gira o seu stock**, comprando limões, açúcar, copos e gelo.  
3. **Observe a previsão do tempo**, pois dias quentes aumentam as vendas! ☀️  
4. **Tome decisões** para expandir o seu lucro e evitar prejuízos.  
5. **O jogo termina após 7 dias**, e o objetivo é ter o maior saldo possível!  

## 🚀 Tecnologias Utilizadas  
- 🔷 **Linguagem:** C
- 🔧 **Compilador:** GCC (MinGW)
- 📝 **Editor de Código:** Notepad++  

## 📥 Como Abrir e Compilar no Notepad++  
1. **Abrir a Linha de Comandos (CMD)**  
   - Clique em **Iniciar** → escreva **cmd** na barra de pesquisa do Windows e abra a aplicação.  
   - Ou pressione as teclas **Windows + R** para abrir.  

2. **Navegar até à Pasta do Projeto**  
   - No CMD, escreva o seguinte comando para verificar a pasta onde você está localizado:  
     ```sh
     cd
     ```
   - Para listar os ficheiros dentro da pasta atual:  
     ```sh
     dir
     ```
   - Para mudar para a pasta do projeto (`projeto_teresa_limonada`), use:  
     ```sh
     cd C:\caminho\para\projeto_teresa_limonada
     ```
     *(Substitua `C:\caminho\para\projeto_teresa_limonada` pelo caminho real onde guardou o seu projeto.)*  

3. **Listar os Ficheiros da Pasta**  
   - Para ver os ficheiros `.c` na pasta:  
     ```sh
     dir *.c
     ```
   - Isto deve mostrar o ficheiro **jogo_limonada.c** na lista.  

4. **Abrir o Código no Notepad++**  
   - Usa o comando:  
     ```sh
     notepad++ jogo_limonada.c
     ```
   - Se o Notepad++ não abrir, pode abrir manualmente:  
     - Vá até **Área de Trabalho** → **Programas** → **Notepad++**  
     - Clique em **Ficheiro > Abrir** e selecione `jogo_limonada.c`.  

5. **Compilar e Executar o Programa**  
   - No CMD, estando dentro da pasta do projeto, use:  
     ```sh
     gcc jogo_limonada.c -o jogo.exe
     ```
   - Isto cria o ficheiro `jogo.exe`, que pode executar com:  
     ```sh
     jogo.exe
     ```
   - O jogo será iniciado diretamente no terminal.  

6. **Criar um Atalho para Compilar e Executar no Notepad++**  
   - No Notepad++, vá a **Executar > Executar... (F5)**.  
   - No campo de comando, escreva:  
     ```sh
     cd C:\caminho\para\projeto_teresa_limonada && gcc jogo_limonada.c -o jogo.exe && jogo.exe
     ```
   - Substitua `C:\caminho\para\projeto_teresa_limonada` pelo caminho real da pasta.  
   - Clique em **Guardar**, dê um nome como **"Compilar e Executar C"**, e atribua um atalho de teclado, por exemplo, `Ctrl + F9`.  
   - Agora, sempre que quiser compilar e correr o jogo, basta pressionar **Ctrl + F9**!  

## 🚀Explicação das funções do jogo

-   **iniciarJogo()**: Esta função começa o jogo e define os valores iniciais, como o orçamento e os itens no inventario (limões, açúcar, copos e gelo).
    
-   **simularDia()**: Cada vez que passa um dia no jogo, esta função é chamada para simular as ações que acontecem no dia. Mostra o inventário, prevê o tempo, permite comprar os ingredientes e define o preço dos copos de limonada que o utilizador deseja e calcular as vendas.
    
-   **mostrarInventario()**: Mostra o estado atual do inventario, mostrando quantos limões, açúcar, copos e gelo tem, além do orçamento que esta disponível.
    
-   **gerirInventario()**: Permite que o jogador compre ingredientes para o seu stock, como limões, açúcar, copos e gelo. O orçamento é atualizado dependendo do que o jogador compra.
    
-   **definirPreco()**: Permite ao jogador definir o preço dos copos de limonada que vai vender.
    
-   **calcularVendas()**: Esta função calcula quantos copos de limonada podem ser vendidos com base na previsão do tempo, o preço definido e a quantidade de ingredientes no inventário.
    
-   **eventosAleatorios()**: Faz eventos aleatórios que afetam o jogo. Por exemplo, uma onda de calor pode aumentar a procura, ou um atraso no fornecedor pode limitar o que o jogador pode receber de ingredientes.
    
-   **exibirResumoFinal()**: No final do jogo, esta função exibe o lucro total e o orçamento final que o jogador teve.
    
-   **limparTela()**: Limpa a tela do terminal, para que a interface do jogo fique mais limpa e sem confusão assim ficando mais bonito.
    
-   **mostrarCreditos()**: Exibe os créditos do jogo, dizendo quem o desenvolveu e informação sobre o projeto.
    
-   **mostrarTutorial()**: Dá um guia ao jogador sobre como jogar. Explica como funcionam as compras, as vendas, o inventário, as previsões do tempo e os eventos aleatórios.
-  **salvarPaginaFinal()**: No final do jogo, mostra o lucro total e o orçamento final numa pagina txt à parte denominada "resultado_final.txt".
