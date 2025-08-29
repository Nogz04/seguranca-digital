### Criando arquivos com dados dentro e mostrando os dados dentro

```txt
vi teste1.txt

www

vi teste2.txt

mail

vi teste3.txt

ftp

cat teste1.txt
cat teste2.txt
cat teste3.txt

```

### Concatenando arquivos com CAT

```txt

vi dominios1.lst

cat teste1.txt teste2.txt teste3.txt > dominios1.lst

```

### Linha do tempo de comandos que utilizei

```txt
┌──(laboratorio㉿lab24dt01)-[/home]
└─$ cd laboratorio
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ ls -la
total 120
drwx------ 16 laboratorio laboratorio  4096 ago 29 08:02  .
drwxr-xr-x  3 root        root         4096 out 15  2024  ..
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024 'Área de trabalho'
-rw-r--r--  1 laboratorio laboratorio   220 out 15  2024  .bash_logout
-rw-r--r--  1 laboratorio laboratorio  5551 out 15  2024  .bashrc
-rw-r--r--  1 laboratorio laboratorio  3526 out 15  2024  .bashrc.original
drwxrwxr-x  2 laboratorio laboratorio  4096 ago 29 07:54  .bully
drwx------ 13 laboratorio laboratorio  4096 out 15  2024  .cache
drwxr-xr-x 17 laboratorio laboratorio  4096 ago 18 19:42  .config
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Documentos
-rw-rw-r--  1 laboratorio laboratorio    40 ago 22 10:51  dominios.lst
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Downloads
-rw-r--r--  1 laboratorio laboratorio 11759 out 15  2024  .face
lrwxrwxrwx  1 laboratorio laboratorio     5 out 15  2024  .face.icon -> .face
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Imagens
drwxr-xr-x  3 laboratorio laboratorio  4096 out 15  2024  .java
drwxr-xr-x  4 laboratorio laboratorio  4096 out 15  2024  .local
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Modelos
drwx------  4 laboratorio laboratorio  4096 out 15  2024  .mozilla
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Músicas
-rw-r--r--  1 laboratorio laboratorio   807 out 15  2024  .profile
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Público
-rw-r--r--  1 laboratorio laboratorio     0 out 15  2024  .sudo_as_admin_successful
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Vídeos
-rw-------  1 laboratorio laboratorio   825 ago 22 10:55  .viminfo
-rw-------  1 laboratorio laboratorio   799 ago 29 07:54  .zsh_history
-rw-r--r--  1 laboratorio laboratorio 10868 out 15  2024  .zshrc
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ pwd
/home/laboratorio
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste1.txt  

[Alterações não gravadas]

Aperte ENTER ou digite um comando para continuar
[Alterações não gravadas]

Aperte ENTER ou digite um comando para continuar
[Alterações não gravadas]

Aperte ENTER ou digite um comando para continuar
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi                       


Aperte ENTER ou digite um comando para continuar
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste1.txt
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste1.txt
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat teste1.txt  
www
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste2.txt
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat teste2.txt
mail
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste3.txt 
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste3.txt
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste3.txt 
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat dominios.lst
google.com
uol.com.br
clubedores.com.br
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat teste1.txt teste2.txt teste3.txt > dominios.lst
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat dominios.lst                                   
www
mail
ftp
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi dominios1.lst
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi              
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi dominios1.lst
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat dominios1.lst
www
mail
ftp


```
# Comandos de Permissões

1 - Permite executar
2 - Permite gravar
3 - Permite leitura

Exemplo:

1 1 1

Representa permissões para:

Owner (Dono) | Grupo (Group) | Outros (Outros)


# Perguntas pro chat? 

└─$ ./busca_subdominios.sh ufn.edu.br

> www.ufn.edu.br -> 200.132.59.110

┌──(laboratorio㉿lab24dt01)-[~]
└─$ ./busca_subdominios.sh host ufn.edu.br

> mail.host has address 52.20.84.62

porque dao diferentes?





