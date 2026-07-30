
# 📂 Organização de Pastas e Arquivos no Terminal

---

## 🎯 Introdução — A Importância da Organização

Organização não é apenas uma questão de estética.  
É uma habilidade essencial em qualquer área profissional — e no desenvolvimento de software isso se torna ainda mais crítico.

Programadores lidam diariamente com:

- Múltiplos arquivos
- Diferentes versões de código
- Documentações
- Recursos de mídia
- Configurações
- Projetos colaborativos

Sem organização, um projeto rapidamente se torna difícil de entender, manter e evoluir.

Uma estrutura bem definida:

- ✅ Facilita leitura e manutenção do código  
- ✅ Reduz erros  
- ✅ Melhora o trabalho em equipe  
- ✅ Aumenta produtividade  
- ✅ Demonstra profissionalismo  

Empresas não avaliam apenas se o código funciona.  
Elas avaliam **como ele está estruturado**.

Aprender a organizar pastas e arquivos desde o início da formação técnica desenvolve:

- Pensamento estruturado  
- Visão de arquitetura  
- Planejamento antes da execução  

Neste material, você aprenderá a organizar arquivos e diretórios usando o terminal no Git Bash (shell Bash, padrão em sistemas Linux).

Mais do que aprender comandos, você estará aprendendo a pensar como um desenvolvedor.



# 🟢 NÍVEL 1 — Estrutura Básica

## Criando uma pasta

```bash
mkdir empresa
````

## Criando múltiplas pastas

```bash
mkdir financeiro RH TI
```

## Criando subpastas automaticamente

```bash
mkdir -p empresa/financeiro
```

---

# 🟡 NÍVEL 2 — Organização Inteligente

## Criando múltiplos departamentos

```bash
mkdir -p empresa/{financeiro,RH,TI}
```

Resultado esperado:

```
empresa
├── financeiro
├── RH
└── TI
```

## Criando subpastas internas

```bash
mkdir -p empresa/{financeiro/{2024,2025},RH,TI}
```

## Criando arquivos organizados

```bash
touch empresa/financeiro/relatorio.txt
```

---

# 🟠 NÍVEL 3 — Automação Simples

## Criando arquivos numerados

```bash
touch relatorio{1..5}.txt
```

## Organizando por tipo de arquivo

```bash
mkdir imagens documentos
mv *.jpg imagens/
mv *.txt documentos/
```

## Criando backup completo

```bash
cp -r empresa empresa_backup
```

---

# 🔵 Estrutura de Projeto Simples

```bash
mkdir -p projeto/{src,docs,assets}
```

Resultado:

```
projeto
├── src
├── docs
└── assets
```

---

# ✍️ Editores de Texto no Terminal

## 📝 Nano (Recomendado para iniciantes)

Abrir arquivo:

```bash
nano arquivo.txt
```

Comandos principais:

* `Ctrl + O` → Salvar
* `Ctrl + X` → Sair

---

## 📝 Vim (Mais avançado)

Abrir arquivo:

```bash
vim arquivo.txt
```

Comandos principais:

* `i` → Modo inserção
* `ESC` → Sair do modo inserção
* `:w` → Salvar
* `:q` → Sair
* `:wq` → Salvar e sair

---

# 🧠 Exercícios de Fixação

---

## 🟢 Exercícios Simples

1. Crie uma pasta chamada `aula`.
2. Dentro dela, crie as pastas:

   * teoria
   * pratica
3. Liste o conteúdo criado.
4. Crie um arquivo chamado `anotacoes.txt` dentro de `teoria`.

---

## 🟡 Exercícios Intermediários

1. Crie a seguinte estrutura usando o menor número possível de comandos:

```
startup
├── backend
├── frontend
└── banco
```

2. Dentro de `backend`, crie:

   * src
   * tests

3. Crie 3 arquivos numerados dentro de `tests`.

4. Faça uma cópia completa da pasta `startup`.

---

## 🟠 Exercícios Avançados (Iniciante Plus)

1. Crie a seguinte estrutura:

```
empresa
├── financeiro
│   ├── 2024
│   └── 2025
├── RH
└── TI
```

2. Dentro de cada pasta principal, crie um arquivo chamado `info.txt`.

3. Crie uma pasta chamada `arquivos_temp` e mova todos os arquivos `.txt` para dentro dela.

4. Faça backup da pasta `empresa`.

---

## 🔵 Desafio Final

Monte esta estrutura com o menor número possível de comandos:

```
projeto_final
├── src
│   ├── components
│   └── services
├── public
└── docs
```

Regras:

* Usar `mkdir -p`
* Criar pelo menos 2 arquivos dentro de `src`
* Criar backup da estrutura

---

# 🏁 Conclusão

Organização de arquivos é a base de qualquer projeto bem estruturado.

Dominar o terminal significa:

* Ter controle do sistema
* Trabalhar com mais eficiência
* Desenvolver pensamento estruturado

> Quem organiza bem arquivos, organiza bem projetos.

