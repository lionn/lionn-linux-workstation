# lionn-linux-workstation

Workstation Linux pessoal provisionada por código, com ambientes para DevOps, desenvolvimento, criação de conteúdo, áudio, música e gaming.

---

## Descrição

Uma workstation Linux pessoal provisionada por código, criada para reunir em um único ambiente as ferramentas que utilizo no meu dia a dia e também para experimentar novas tecnologias.

O projeto nasceu da ideia de transformar um computador antigo em uma estação de trabalho completa utilizando Debian GNU/Linux, mantendo a configuração organizada, documentada e, sempre que possível, automatizada.

---

## Objetivo

A ideia é construir uma workstation que possa ser reproduzida e configurada através de scripts e documentação, evitando depender de uma configuração feita manualmente do zero toda vez que o sistema precisar ser reinstalado.

O ambiente será utilizado para diferentes atividades, incluindo:

- DevOps e infraestrutura
- Desenvolvimento web
- Desenvolvimento e administração de Magento 2
- Criação e edição de vídeo
- Áudio e produção musical
- Steam e jogos
- Emulação e retrogaming

O projeto também funciona como um laboratório pessoal para testar ferramentas, configurações e automações no Linux.

---

## Ambiente

O sistema operacional principal será o **Debian GNU/Linux**, instalado diretamente no hardware da workstation.

A configuração será construída gradualmente e documentada conforme cada etapa for sendo testada no ambiente real.

---

## Estrutura do projeto

```text
lionn-linux-workstation/
├── .github/
│   └── workflows/
├── configs/
│   ├── audio/
│   ├── devops/
│   ├── gaming/
│   ├── magento/
│   └── video/
├── docs/
├── scripts/
├── assets/
├── .gitignore
└── README.md
```

---

## Áreas do ambiente

### DevOps

Ambiente voltado para estudos, desenvolvimento e testes relacionados a:

- Linux
- Git
- Docker
- Docker Compose
- Terraform
- automação
- Bash
- Python
- CI/CD

### Desenvolvimento

Ambiente para desenvolvimento e testes de aplicações web, incluindo ferramentas e tecnologias utilizadas no dia a dia.

### Magento 2

Ambiente específico para desenvolvimento, testes e laboratório com Magento 2.

A workstation também servirá como ambiente local complementar aos projetos Magento e DevOps da Lionn.

### Criação de conteúdo

Ferramentas para edição de vídeo, processamento de áudio, criação de imagens, animação e outras atividades relacionadas à produção de conteúdo.

### Áudio e música

Ambiente para experimentação e produção musical utilizando software, incluindo instrumentos virtuais, MIDI, sintetizadores, samplers e efeitos de áudio.

### Gaming

Ambiente para jogos utilizando Steam e outras ferramentas compatíveis com Linux.

Também serão utilizados emuladores para diferentes plataformas clássicas, mantendo os arquivos de jogos e BIOS fora do repositório quando forem protegidos por direitos autorais.

---

## Automação

Sempre que possível, a configuração da workstation será realizada através de scripts.

A intenção não é simplesmente criar uma lista de programas para instalar, mas transformar a configuração do ambiente em um processo organizado e reproduzível.

A evolução esperada do projeto segue aproximadamente esta sequência:

```text
Debian
   ↓
Configuração base
   ↓
DevOps
   ↓
Desenvolvimento
   ↓
Magento
   ↓
Vídeo
   ↓
Áudio e música
   ↓
Steam
   ↓
Retrogaming
```

Cada etapa será testada na workstation antes de ser considerada concluída.

---

## Documentação

A documentação será construída junto com o ambiente.

Os procedimentos ficam organizados em:

```text
docs/
```

Cada documento representa uma etapa da configuração da workstation.

---

## Status

**Em desenvolvimento.**

A workstation será construída gradualmente em hardware real, e novas ferramentas, configurações e automações serão adicionadas conforme a necessidade e evolução do projeto.
