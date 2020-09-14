# linux
# Guia de Linux para iniciantes 

# Comandos básicos na Linha de Comando
Comandos fundamentais do Linux/Unix para o aprendiz de linha de comando Linux/Unix. Se você for experiente com Linux/Unix: você provavelmente já dominou estes comandos. Caso contrário: você está no lugar certo.

Nota: Alguns dos exemplos abaixo pressupõem arquivos e caminhos que podem não corresponder à sua instalação de sistemas e ferramentas particulares.

Onde Adquirir

Estas ferramentas são instaladas nativamente na maioria das distribuições Unix/Linux, assim como no OS X.
---
Noções básicas

# Função autocompletar com TAB:</br>

As pessoas que são novas na linha de comando Unix/Linux frequentemente tentam digitar tudo na mão. Isto pode até funcionar bem se você digitar rápido e com precisão suiça.
O que não é verdade para a maioria de nós sendo muito melhor usar a função autocompletar usando a tecla TAB.

Note que o Windows PowerShell também suporta o preenchimento com TAB, mas ele lida com a ambigüidade de forma diferente. 

Digite o seguinte, e então pressione a tecla <TAB>:
```
$ cat /etc/pas
```

Em seguida, pressione <TAB>.

Note que ela se autocompleta para /etc/passwd.

Agora tente a tabulação com ambigüidade:
```
$ cd ~/Do
```

Depois pressione <TAB>>TAB>.

Note que ela oferece duas opções: Documentos/ Downloads/.

Agora adicione um "w" e pressione <TAB>:
```
$ cd ~/Dow
```
Pressione <TAB>. Ela se autocompleta para ~/Downloads/.

cat
Mostrar um arquivo:
```
$ cat example.txt
```

Concatenar (cat) FileA.txt e FileB.txt, criar FileC.txt:

```
$ cat FileA.txt FileB.txt > FileC.txt
```

---
cd
Change Directory (Mudar Diretório) (cd) para o diretório /tmp:
```
$ cd /tmp
```


Mudança para o diretório home. Os seguintes comandos são equivalentes para o "aluno".
usuário: "~" significa diretório home (por exemplo: /home/aluno):
```
$ cd
$ cd ~
$ cd /home/student
```

Mudança para o diretório principal. Por exemplo: se você estiver em /tmp/subdiretório/, isto
muda seu diretório de trabalho para /tmp/:
```
$ cd ..
```

---
echo
Imprimir (echo) a string "Cylon":
```
$ echo Cylon
```

Criar ou sobrescrever o arquivo exemplo.txt, contendo a string "Cylon":
```
$ echo Cylon > example.txt
```

Acrescentar a string "Cylon" ao arquivo exemplo.txt:
```
$ echo Cylon >> example.txt
```

---
ls
Liste os arquivos no diretório atual (equivalente ao comando "dir" no cmd.exe):

```
$ ls
```

Liste os arquivos no diretório atual, saída longa (-l), todos os arquivos incluindo os arquivos "ocultos" que começam com um "." (-a):
```
$ ls -la
```

Liste os arquivos no diretório atual, saída longa (-l), todos os arquivos (-a), ordenar por hora (-t):
```
$ ls -lat
```

Liste os arquivos no diretório atual, saída longa (-l), todos os arquivos (-a), reverso (-r) ordenar por hora (-t):
```
$ ls -lart
```

---
rede
Mostrar a configuração da interface de rede:

```
$ ifconfig
```

Mostrar a configuração da interface de rede usando "ip":
```
$ ip a
```

Reiniciar a rede:
```
$ sudo /etc/init.d/networking restart
```

---
passwd
Altere sua senha:
```
$ passwd
```

---
ping
pingar um host para sempre (até que o CTRL-C seja pressionado), ver se ele está no ar (e não filtrado):
```
$ ping 8.8.8.8
```

pingar um host 3 vezes, ver se ele está no ar (e não filtrado):
```
$ ping -c3 8.8.8.8
```

---
pwd
Print Working Directory (Imprimir diretório de trabalho) (pwd), mostrar o diretório atual:
```
$ pwd
```

---
sudo
Executar um comando como root:
```
$ sudo comando
```

Abrir uma shell como root:
```
$ sudo bash
```

extraído de SANS - Linux 101 Command Line Cheat Sheet
