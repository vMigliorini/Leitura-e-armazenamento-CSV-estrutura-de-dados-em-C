![C](https://img.shields.io/badge/C-99-blue?logo=c)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-concluído-brightgreen)

# Tabela Nutricional em C

Programa de terminal que lê uma base de dados nutricional em CSV, armazena os alimentos em structs e permite consultar e ordenar os dados por diferentes critérios — energia, proteína, carboidrato, umidade e suas relações.

---

## Pré-requisitos

- GCC 9+ (ou qualquer compilador C99)
- CMake 3.x *(opcional)*

## Instalação

```bash
git clone https://github.com/vMigliorini/Leitura-e-armazenamento-CSV-em-estrutura-de-dados.git
cd Leitura-e-armazenamento-CSV-em-estrutura-de-dados
gcc main.c -o tabela_nutricional
```

## Uso

```bash
./tabela_nutricional
```

> `alimentos.txt` deve estar na mesma pasta do executável.

```
** MENU DE OPCOES **
[1]  Listar todas as categorias
[2]  Alimentos de uma categoria em ordem alfabética
[3]  Todos os alimentos de uma categoria por energia (decrescente)
[4]  N alimentos com maior umidade
[5]  N alimentos com maior energia
[6]  N alimentos com maior proteína
[7]  N alimentos com maior carboidrato
[8]  N alimentos com maior relação Energia/Proteína
[9]  N alimentos com maior relação Energia/Carboidrato
[10] Sair
```

## Estrutura do projeto

```
├── main.c          # Código-fonte principal
├── alimentos.txt   # Base de dados nutricional (CSV)
├── CMakeLists.txt  # Build alternativo com CMake
└── README.md
```

## Observação

O locale está configurado para Windows (`Portuguese_Brazil.1252`). Em Linux/macOS, altere para `pt_BR.UTF-8` na linha `setlocale` antes de compilar.

---

Desenvolvido por [@vMigliorini](https://github.com/vMigliorini)
