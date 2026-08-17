# Instalando o Debian 13

Este documento descreve o processo de instalação do **Debian GNU/Linux 13** na workstation que será utilizada pelo projeto `lionn-linux-workstation`.

A instalação será realizada diretamente no hardware da workstation, utilizando um pendrive inicializável criado no Windows.

---

## Objetivo

Instalar uma versão limpa do Debian 13 para servir como base da workstation.

Após a instalação, as demais configurações do ambiente serão realizadas gradualmente através de documentação e scripts.

---

## Pré-requisitos

Para realizar esta etapa serão necessários:

- Um computador com Windows para preparar o pendrive
- Um pendrive com espaço suficiente para a ISO
- A ISO do Debian 13
- Rufus
- O computador que será utilizado como workstation
- Acesso à BIOS/UEFI ou Boot Menu do computador

---

## 1. Baixar a ISO do Debian

A ISO deve ser obtida através dos canais oficiais do projeto Debian.

Após o download, verificar se o arquivo foi baixado corretamente antes de utilizá-lo para criar o pendrive inicializável.

---

## 2. Baixar o Rufus

No Windows, utilizar o Rufus para criar o pendrive inicializável.

O Rufus será utilizado somente para preparar o dispositivo USB. O sistema operacional que será instalado na workstation será o Debian GNU/Linux.

---

## 3. Preparar o pendrive

Conectar o pendrive ao computador Windows e abrir o Rufus.

Selecionar:

- O pendrive correto em **Dispositivo**
- A ISO do Debian em **Seleção de boot**

A configuração da tabela de partição depende do firmware do computador que receberá o Debian.

### Computador com UEFI

Preferencialmente:

```text
Esquema de partição: GPT
Sistema de destino: UEFI
```

### Computador com BIOS Legacy

Em computadores que utilizam BIOS Legacy:

```text
Esquema de partição: MBR
Sistema de destino: BIOS
```

> A escolha deve ser feita de acordo com o modo de inicialização configurado no computador que receberá a workstation.

---

## 4. Inicializar o computador pelo pendrive

Antes de iniciar a instalação, verificar na BIOS/UEFI qual modo de inicialização está sendo utilizado.

Não é necessário alterar outras configurações da BIOS/UEFI neste momento.

Após finalizar a criação do pendrive:

1. Desligar o computador que receberá o Debian.
2. Conectar o pendrive.
3. Ligar o computador.
4. Abrir o **Boot Menu** ou a **BIOS/UEFI**.
5. Selecionar o dispositivo USB.
6. Iniciar o instalador do Debian.

A tecla utilizada para acessar o Boot Menu varia conforme o fabricante da placa-mãe ou computador.

Algumas teclas comuns são:

```text
F12
F11
F8
Esc
Del
```

---

## 5. Instalar o Debian

No instalador do Debian:

1. Selecionar o idioma.
2. Selecionar a localização.
3. Configurar o teclado.
4. Configurar a rede.
5. Definir o nome da máquina.
6. Configurar o usuário.
7. Configurar o particionamento do disco.
8. Selecionar os componentes necessários.
9. Instalar o carregador de inicialização.
10. Finalizar a instalação.

### Particionamento

Como esta workstation será dedicada ao projeto, o particionamento será definido durante a instalação considerando o hardware disponível.

Antes de confirmar qualquer alteração no disco, verificar cuidadosamente se o dispositivo selecionado é realmente o disco destinado à workstation.

> **Atenção:** o particionamento pode apagar os dados existentes no disco selecionado.

---

## 6. Primeiro boot

Após a instalação:

1. Remover o pendrive.
2. Reiniciar o computador.
3. Confirmar que o Debian inicia normalmente.
4. Realizar o login.
5. Verificar a conexão de rede.
6. Confirmar o funcionamento básico do hardware.

Neste momento, a workstation ainda não possui as ferramentas de DevOps, desenvolvimento, Magento, criação de conteúdo ou gaming.

Esses ambientes serão configurados nas etapas seguintes.

---

## 7. Hardware utilizado

As informações específicas do hardware serão registradas após a instalação e confirmação dos componentes presentes na workstation.

Exemplo:

```text
Modelo: Dell XPS 8900
Processador: Intel Core i7
Memória RAM: [a confirmar]
Armazenamento: [a confirmar]
GPU: [a confirmar]
Modo de inicialização: [UEFI ou Legacy]
```

> Os dados acima devem ser preenchidos somente após serem confirmados no hardware.

---

## 8. Próxima etapa

Após confirmar que o Debian está funcionando corretamente, seguir para:

```text
docs/
├── 01-instalando-o-debian.md
├── 02-configurando-o-sistema.md
├── 03-configurando-a-rede.md
└── ...
```

A configuração da workstation será construída gradualmente, sendo testada no hardware real antes de ser transformada em automação.

---

## Status

**Em desenvolvimento.**

Esta documentação será atualizada conforme a instalação for realizada e os procedimentos forem validados na workstation.
