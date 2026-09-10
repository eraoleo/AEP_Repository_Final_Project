# AEP_Repository_Final_Project
# PSE em Ação — Sistema de Planejamento e Acompanhamento de Ações de Saúde na Escola

Atividade de Estudo Prático (AEP) — 2º semestre de 2026
Universidade Cesumar (UNICESUMAR) — Curso de Engenharia de Software

Disciplinas integradas: Produção Textual, Algoritmos e Lógica de Programação, Engenharia de Software e Linguagem e Técnicas de Programação.

## Integrantes

| Nome | RA |
|---|---|
| Leonardo de Souza Caires | 26006198-2 |
| Larissa Geovanna Mourão Silva | 26012271-2 |

## Sobre o projeto

O Programa Saúde na Escola (PSE), instituído pelo Decreto nº 6.286/2007, articula as áreas da Saúde e da Educação no desenvolvimento de ações coletivas nas escolas públicas. Na rotina das equipes intersetoriais, o planejamento dessas ações costuma ficar disperso entre anotações, formulários e planilhas separadas, o que dificulta localizar o que está programado, verificar o que foi concluído, identificar cancelamentos e consolidar quantos participantes foram atendidos.

Este projeto desenvolve uma aplicação de terminal em linguagem C para registrar, consultar e acompanhar essas ações, gerando informações consolidadas de participação.

**Questão norteadora:** como uma aplicação desenvolvida em linguagem C pode auxiliar uma equipe escolar e de saúde a planejar, registrar e acompanhar ações coletivas do Programa Saúde na Escola, apresentando informações claras e preservando a privacidade dos estudantes?

## Funcionalidades previstas

| Código | Funcionalidade |
|---|---|
| RF01 | Cadastrar ação (código, escola, tema, data prevista, público-alvo, responsável, quantidade prevista) |
| RF02 | Listar todas as ações cadastradas |
| RF03 | Pesquisar ações por código, escola ou tema |
| RF04 | Atualizar situação (planejada / realizada / cancelada) e registrar participação efetiva |
| RF05 | Gerar resumo geral com totais por situação e percentual de participação |
| RF06 | Validar entradas (código duplicado, quantidade negativa, campo vazio, opção inexistente) |
| RF07 | Controlar o menu principal por estrutura de repetição |
| RF08 | Tratar o limite de armazenamento |

## Limites éticos

O sistema utiliza **exclusivamente dados fictícios e informações coletivas** sobre as ações. Não armazena nome, diagnóstico, prontuário, condição clínica ou qualquer dado sensível individual de estudantes, e não realiza diagnóstico, triagem médica, prescrição ou recomendação de tratamento.

## Tecnologia

- Linguagem C padrão, apenas bibliotecas nativas
- Compilação com GCC
- Armazenamento em memória durante a execução (vetor de registros, capacidade de 100 ações)

## Estrutura do repositório

```
pse-em-acao/
├── README.md
├── docs/
│   ├── AEP_Etapa1.pdf
│   ├── fluxograma-geral.png
│   ├── fluxograma-cadastro.png
│   └── pseudocodigos.md
└── src/
    └── (código-fonte em C — 2ª etapa)
```

## Compilação e execução

Instruções a serem incluídas na 2ª etapa, junto com o código-fonte:

```bash
gcc src/main.c -o pse
./pse
```

## Estado atual

- [x] **1ª etapa** — documento escrito: contextualização, requisitos, riscos, fluxogramas, pseudocódigos e planejamento das sprints
- [ ] **2ª etapa** — implementação em C, casos de uso, manual do usuário e apresentação em vídeo

## Referências

- BRASIL. Decreto nº 6.286, de 5 de dezembro de 2007. Institui o Programa Saúde na Escola — PSE e dá outras providências.
- BRASIL. Ministério da Saúde. Portaria Interministerial nº 1.055, de 25 de abril de 2017.
- LOPES, I. E.; NOGUEIRA, J. A. D.; ROCHA, D. G. Eixos de ação do Programa Saúde na Escola e Promoção da Saúde: revisão integrativa. *Saúde em Debate*, v. 42, n. 118, p. 773-789, 2018.
- SOUSA, M. C. de; ESPERIDIÃO, M. A.; MEDINA, M. G. A intersetorialidade no Programa Saúde na Escola. *Ciência & Saúde Coletiva*, v. 22, n. 6, p. 1781-1790, 2017.
