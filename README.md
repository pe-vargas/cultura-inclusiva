# Cultura Inclusiva

**Universidade Tuiuti do Paraná | 2025**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)

## Sobre o trabalho

Projeto desenvolvido em dupla como atividade acadêmica da disciplina de **Interface Humano e Computador**, do curso de Análise e Desenvolvimento de Sistemas da Universidade Tuiuti do Paraná (UTP).

O trabalho consiste em uma aplicação web cultural acessível para pessoas com deficiência, chamada **Cultura Inclusiva**. A aplicação divulga eventos culturais (teatro, exposições e cinema) e permite filtrá-los pelo tipo de acessibilidade oferecido.

O projeto segue as diretrizes da **WCAG 2.1** e boas práticas de design inclusivo. O processo completo (storytelling, personas, fluxo de tarefas, protótipos e avaliação da interface) está na [documentação do projeto](documentacao/documentacao-do-projeto.pdf).

## Objetivos

- Divulgar eventos culturais acessíveis;
- Permitir filtros por tipo de acessibilidade;
- Exibir um mapa com marcadores de eventos;
- Oferecer recursos visuais inclusivos (dislexia, daltonismo e tema escuro);
- Facilitar o acesso à cultura para pessoas com deficiência.

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript (puro, sem frameworks)
- Tailwind CSS, via CDN (somente na tela de login)
- Fonte OpenDyslexic, via web font

## Telas do site

| Tela | Arquivo | Descrição |
|---|---|---|
| Login e cadastro | `index.html` | Formulários em abas, com validação dos campos e mensagens de sucesso e erro |
| Eventos | `eventos.html` | Lista de eventos com filtro de acessibilidade, favoritos, detalhes e configurações visuais |
| Mapa | `mapa.html` | Marcadores numerados sobre o mapa e cartões dos eventos com rolagem horizontal |

## Funcionalidades

### Login e cadastro
- Alternância entre as abas **Fazer Login** e **Criar Conta**;
- Validação de e-mail, de senha com no mínimo 6 caracteres e de confirmação de senha;
- Mensagens de sucesso e erro;
- Após o login, redirecionamento para a tela de eventos.

### Eventos
- Filtro por recurso de acessibilidade: **Intérprete de Libras**, **Audiodescrição**, **Acessibilidade Motora** e **Sessão Azul (TEA)**;
- Etiquetas com ícone em cada evento (♿ Física, 👋 Libras, 🎧 Áudio, 🧩 TEA);
- Detalhes expansíveis, com imagem, preço e descrição;
- Botão para salvar eventos nos favoritos;
- Barra de navegação inferior com ícones.

### Configurações de acessibilidade
- **Modo escuro**;
- **Modos de daltonismo**: protanopia, deuteranopia e tritanopia;
- **Facilidade de leitura**: fonte OpenDyslexic para pessoas com dislexia;
- As preferências escolhidas ficam salvas no navegador (`localStorage`), assim como os eventos favoritos.

### Mapa
- Marcadores numerados posicionados sobre uma imagem de mapa;
- Cartões flutuantes dos eventos, com rolagem horizontal;
- Ao clicar em um marcador ou cartão, o evento correspondente é destacado.

## Documentação

A documentação do projeto contém:

| Seção | Conteúdo |
|---|---|
| Fundamentos teóricos | Diretrizes de acessibilidade da WCAG 2.1 |
| Storytelling | Contexto de uso e mapa de personas |
| Personas | Maria Andrade (motora), Roberto Lima (visual e dislexia), Ana Paula (auditiva) e Gabriel (TEA) |
| Fluxo de tarefas | Caminho básico, caminhos alternativos, exceções e mapa de navegação |
| Protótipos | Protótipo de alta fidelidade, representado diretamente no código |
| Avaliação da interface | Heurísticas de Nielsen e critérios do W3C |

## Estrutura do projeto

```text
index.html
eventos.html
mapa.html

documentacao/
└── documentacao-do-projeto.pdf
```

A pasta `documentacao/` possui seu próprio README: [documentacao](documentacao/README.md)

## Como executar

Não há necessidade de instalação. Basta baixar o repositório e abrir o arquivo `index.html` no navegador.

**Importante:** o site carrega o Tailwind CSS, a fonte OpenDyslexic e as imagens dos eventos pela internet, então é necessário estar conectado.

## Limitações

- O login e o cadastro são uma **simulação**: não há servidor nem banco de dados, e nenhuma conta é realmente criada;
- O mapa é uma imagem com marcadores posicionados em porcentagem, sem serviço de mapas real e sem rotas;
- Os eventos são fictícios e estão definidos no próprio código;
- O link **Ver Detalhes** do mapa aponta para `index.html`, e não para `eventos.html`;
- Faltam os atributos `aria-label` e outros recursos para leitores de tela, apontados como ponto de melhoria na documentação.

## Integrantes

- Alexandre Mehes
- Pedro Dambiski de Vargas

## Informações acadêmicas

| Informação | Detalhes |
|---|---|
| Instituição | Universidade Tuiuti do Paraná (UTP) |
| Curso | Análise e Desenvolvimento de Sistemas |
| Disciplina | Interface Humano e Computador |
| Professora | Patricia Rucker de Bassi |
| Ano | Segundo Semestre de 2025 |
| Tipo | Trabalho acadêmico em dupla |

---

**Observação:** Este repositório tem finalidade acadêmica e documental, reunindo os arquivos e a documentação desenvolvidos para a atividade proposta na disciplina. Os eventos, locais e preços apresentados são fictícios.
