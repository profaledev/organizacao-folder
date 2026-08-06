# 🚀 Guia Passo a Passo: Como Criar Scripts Executáveis (.bat e .sh)

Criar scripts é uma excelente forma de automatizar tarefas repetitivas e entender como o sistema operacional funciona por baixo dos panos. Este material foi estruturado de forma direta e didática, ideal para ser compartilhado em plataformas de ensino e ser utilizado como guia prático.

---

## 🪟 Parte 1: Criando um Script no Windows (.bat)

Os arquivos `.bat` (Batch) são scripts nativos do Windows. Eles leem e executam comandos em sequência no Prompt de Comando (CMD).

### Passo 1: Abrir o editor de texto
Você não precisa de ferramentas complexas. Abra o **Bloco de Notas** (Notepad) ou o seu editor de código preferido (como o VS Code).

### Passo 2: Escrever o código
Digite o seguinte código de exemplo. A primeira linha (`@echo off`) serve para deixar a tela limpa, escondendo os caminhos das pastas durante a execução.

```bat
@echo off
cls
echo Ola, Mundo do Terminal Windows!
echo.
echo Pressione qualquer tecla para finalizar...
pause > nul
```

### Passo 3: Salvar o arquivo corretamente (Atenção aqui!)
1. Vá em **Arquivo > Salvar Como...**
2. Em **Tipo**, é obrigatório mudar de "Documentos de texto (*.txt)" para **"Todos os arquivos (*.*)"**.
3. No **Nome do arquivo**, digite o nome desejado seguido da extensão, por exemplo: `meu_script.bat`.
4. Clique em **Salvar**.

### Passo 4: Executar o script
Vá até a pasta onde você salvou o arquivo. Você notará que o ícone dele tem uma engrenagem. Basta dar um **duplo clique** e o terminal abrirá executando o seu código automaticamente.

---

## 🐧 Parte 2: Criando um Script no Linux / macOS (.sh)

Os arquivos `.sh` são scripts em Shell (geralmente Bash), o interpretador de comandos padrão da maioria das distribuições Linux e do macOS. 

### Passo 1: Abrir o terminal e o editor
Abra o terminal do sistema. Você pode criar o arquivo diretamente por lá usando um editor de texto via linha de comando, como o `nano`.
Digite:
```bash
nano meu_script.sh
```

### Passo 2: Escrever o código
A primeira linha de um script Linux **sempre** deve indicar qual programa vai interpretar o código. Isso se chama *Shebang* (`#!/bin/bash`).

```bash
#!/bin/bash
clear
echo "Olá, Mundo do Terminal Linux/macOS!"
echo ""
read -p "Pressione ENTER para finalizar a execucao..."
```

### Passo 3: Salvar o arquivo
* Se estiver usando o **nano**: Pressione `Ctrl + O` (para salvar), confirme com `ENTER` e depois `Ctrl + X` (para sair do editor).
* Se estiver usando uma interface gráfica como o VS Code, apenas salve o arquivo normalmente garantindo o final `.sh`.

### Passo 4: Dar permissão de execução (O Passo Crítico)
Diferente do Windows, no Linux um arquivo de texto recém-criado não tem permissão de segurança para rodar como um programa. É preciso autorizar. No terminal, digite:
```bash
chmod +x meu_script.sh
```

### Passo 5: Executar o script
Agora que ele tem permissão de execução, você o inicia chamando-o com o `./` na frente (que significa "rode este arquivo que está no diretório atual").
```bash
./meu_script.sh
```

---
**💡 Dica de Ouro para a Sala de Aula:** 
Se os scripts estiverem sendo escritos em máquinas Windows (no VS Code, por exemplo) para depois serem testados em um servidor ou ambiente Linux, atenção à quebra de linha! O Windows usa o padrão `CRLF` e o Linux usa `LF`. Se o script `.sh` der erro de caracteres invisíveis, basta alterar a quebra de linha para `LF` no canto inferior direito do VS Code.
