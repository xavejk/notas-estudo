# notas-estudo
Minhas notas de estudos do Téc. SENAC
 
markdown
 
## Configurando git
 
para utilizar o git na minha máquina eu preciso configurar determinados passos e comandos, sendo eles:
 
1° abrir a aba do Windows e digitar "CMD"
 
2° digitar:
```bash
git config --global user.name "meu nome"
```
3° enter
 
4° digitar
```bash
git config --global user.email "meu email do GitHub"
```
5° enter
 
## SSH- Como configurar a máquina para o GitHub
 
1° verificar se há chave SSH com o comando:
```bash
ls -al ~/.ssh
```
2° abrir o git bash e criar nova chave com o comando:
```bash
ssh-keygen -t ed25519 -C "meu email do GitHub"
```
3° enter 4x
 
4° digitar
```bash
eval "$(ssh-agent -s)"
ssh-add ~/ .ssh/id (tab)
```
5° enter
 
6° copiar chave ssh com o comando:
```bash
clip < ~/.ssh/id(tab).(tab)
```
7° entre no GitHub -> configurações -> SSH => nova chave -> cole a chave
 
8° testar conexão com o comando:
```bash
ssh -T git@github.com
```
## Como criar um repositório no GitHub
 
Repositório é um projeto de git e para criar um é necessário os seguintes passos:
 
abrir o GitHub -> clicar na foto de perfil no canto superior direito -> selecionar repositórios -> clique em "New" no canto superior direito -> dê um nome ao repositório -> crie uma descrição -> defina se será público ou privado -> sempre ative o README
 
## Como clonar o repositório
 
abrir um repositório -> clicar em "<> code" -> selecionar "SSH" -> copiar -> abrir o Git blash -> digitar :
```bash
cd 'nome de uma pasta existente'
```
-> enter -> digitar:
```bash
git clone (clicar botão direito e selecionar "paste")
```
-> enter 2x -> digitar:
```bash
cd 'nome do repositório'
```
-> enter -> digitar:
```bash
code .
```
-> enter