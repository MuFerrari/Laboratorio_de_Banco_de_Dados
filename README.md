# 🗄️ Laboratório de Banco de Dados (LBD) 🗄️

<div align="center">
  <img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white" alt="Oracle">
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="SQL">
</div>

<div align="justify">

  <br></br>
  
  Bem-vindo ao meu repositório de Laboratório de Banco de Dados! Este diretório documenta a minha evolução técnica, os conceitos teóricos estudados e os projetos práticos de modelagem, segurança e otimização de dados desenvolvidos durante a disciplina.
  
  <br></br>
  
  
  ## 🧠 O Que Aprendi Até Aqui (Conceitos Técnicos)
  
  A construção dos **Projetos presentes no Diretório** permitiu a consolidação dos seguintes pilares de Banco de Dados Relacional:
  
  1. **Modelagem Relacional e Normalização**
     * Compreensão do fluxo completo de design, desde o Modelo Conceitual (DER) até o Modelo Lógico. 
     * Aplicação das três Formas Normais (1FN, 2FN, 3FN) para evitar redundâncias, garantir atomicidade dos dados, eliminar dependências parciais em chaves compostas e remover dependências transitivas, garantindo a integridade das informações do sistema.

  2. **Integridade Estrutural (Constraints)**
     * Definição rigorosa da estrutura de tabelas utilizando DDL, assegurando relacionamentos corretos através de Chaves Primárias (PK) e Chaves Estrangeiras (FK). 
     * Aplicação de restrições de validação (`UNIQUE`, `NOT NULL` e `CHECK`) para impedir dados inconsistentes em nível de banco, como CPFs duplicados, valores financeiros negativos, quilometragem de devolução menor que a de retirada ou referências a registros inexistentes.

  3. **Segurança de Dados e Controle de Acesso**
     * Garantia da Tríade CIA (Confidencialidade, Integridade e Disponibilidade) no banco de dados. 
     * Utilização de *Views* convencionais para aplicar restrições de linhas e ocultação de colunas sensíveis, aliadas à concessão de privilégios (`GRANT`/`REVOKE`), implementando o princípio do menor privilégio sem expor as tabelas-base aos usuários.
  
  4. **Otimização e Views Materializadas**
     * Entendimento da diferença de arquitetura entre uma *View* (que armazena apenas a consulta lógica em memória) e uma *Materialized View* (que armazena os dados fisicamente no disco).
     * Uso de visões materializadas para ganho de desempenho em agregações analíticas (como relatórios diários de faturamento) através da criação de índices e políticas de atualização automática transacional (`REFRESH FAST ON COMMIT`).
  
  <br></br>
  
  ## 📂 Arquiteturas e Estruturas
  Os projetos adotam boas práticas de scripts SQL, dividindo a estruturação e a manipulação dos dados de forma semântica:
  * **Scripts DDL (Data Definition Language)**: Responsáveis por criar as tabelas e aplicar todas as restrições (`Constraints`) do modelo lógico.
  * **Scripts DML (Data Manipulation Language)**: Responsáveis pela população da massa de testes no sistema, garantindo simulações reais de negócio.
  * **Scripts DQL (Data Query Language)**: Arquivos com consultas analíticas complexas combinando múltiplas tabelas (`JOIN`, `LEFT JOIN`), agregações (`SUM`, `COUNT`), tratamentos de dados nulos (`NVL`) e ordenações (`GROUP BY`).
  
  <br></br>
  
  ## ⚙️ Como Executar os Projetos
  
  1. Clone este repositório: `git clone <URL_DO_SEU_REPOSITORIO>`
  2. Abra seu ambiente gerenciador de banco de dados (ex: Oracle SQL Developer).
  3. Execute primeiramente o script de DDL para gerar as tabelas.
  4. Execute os scripts DML para popular o banco de dados.
  5. Teste as lógicas de segurança (Views) e rode os testes de restrições previstos na documentação.
  
  <br></br>
  
  ## 🛠️ Tecnologias Utilizadas
  * **Linguagem:** SQL;
  * **SGBD:** Oracle Database 19c/21c;
  * **Conceitos Focais:** Segurança, Performance, DDL/DML, Normalização e Constraints;
</div>
