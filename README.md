# Sistema de Separação Logística (Sem Papel)

## 1. Contexto
Na empresa onde trabalho, usamos coletores para fazer a separação de produtos no setor logístico. Porém, ainda usamos folhas A4 para anotar os ganhos, o que o patrão quer eliminar. Por isso, tive a ideia de criar um sistema digital que substitua esse processo no coletor.

## 2. Objetivo
Criar um sistema simples onde os operadores (coletores) possam registrar os dados da separação diretamente, sem uso de papel, e o encarregado possa visualizar tudo de forma organizada.

## 3. Funcionalidades

### 3.1 Parte dos Operadores (Tela de Registro)
- Login individual para cada operador.
- Registro manual das informações:
  - Número de produção.
  - Para cada um dos 8 produtos separados:
    - Nome do produto.
    - Lote.
    - Quantidade separada (ganho).
- A data do registro é gerada automaticamente.
- Os dados são salvos no banco de dados associados ao usuário.

### 3.2 Parte do Encarregado (Tela de Administração)
- Visualização resumida de todas as separações:
  - Usuário.
  - Número de produção.
  - Data.
  - Total de itens.
  - Opção de ver detalhes.
- Visualização detalhada ao clicar em “Ver Detalhes”:
  - Nome do produto.
  - Lote.
  - Ganho.
- Funcionalidades adicionais:
  - Filtragem por data e por usuário.
  - Exportação de relatórios (PDF ou Excel).
  - (Opcional) Edição ou exclusão de registros.

## 4. Estrutura Técnica

### 4.1 Banco de Dados
- **Tabela usuários**: para login e identificação dos coletores.
- **Tabela registros_producao**: armazena cada produto separado, com número de produção, produto, lote, ganho, data e usuário.

### 4.2 Tecnologias Utilizadas
- Front-end: React (mesmo usado na empresa).
- Estilo: Tailwind CSS.
- Banco de dados: Supabase ou PostgreSQL.
- Futuramente: Integração com o sistema Sankhya.

## 5. Benefícios Esperados
- Eliminação do uso de papel, digitalizando o processo.
- Registro preciso e confiável da separação feita por cada operador.
- Facilitação do acompanhamento e controle por parte do encarregado.
- Melhoria na produtividade e transparência da operação.

---

**Autor:** Vicente  
**Data:** 2025-06-01  
