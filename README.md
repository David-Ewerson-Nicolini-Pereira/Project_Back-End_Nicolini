### A complexidade teórica de diversas áreas de estudo com a praticidade de uma implementação que possa ser gerenciada individualmente.

O projeto proposto é um **Sistema de Gerenciamento de Projetos e Riscos Pessoais Simplificado (Mini-PMO Pessoal)**.

Este projeto, embora *complexo em conteúdo* (por forçar a aplicação de conceitos de múltiplas disciplinas, desde o planejamento estratégico até a codificação e modelagem), pode ser *simples de montar e realizar* se a implementação for mantida em um ambiente controlado, como um aplicativo de console ou desktop local (sem a necessidade de infraestrutura de rede complexa ou implantação em nuvem).

## Projeto: Mini-PMO Pessoal (Gerenciamento Integrado de Tarefas e Riscos)

O objetivo é criar um sistema que permita ao usuário (você) planejar, executar e monitorar tarefas, com foco especial na identificação e mitigação de riscos.

---

### **Fase 1: Concepção e Gerenciamento Estratégico** (Empreendedorismo e G.P. - Iniciação)

Esta fase exige a aplicação de mentalidade empreendedora e de iniciação de projetos.

1.  **Modelo de Negócio (Canvas e PN):** Crie um **Business Model Canvas** simplificado onde o "cliente" e o "usuário final" são você mesmo.
    *   **Proposta de Valor:** Otimizar a gestão de tempo e aumentar a eficácia na conclusão de projetos pessoais, fornecendo ferramentas de análise de risco e caminho crítico.
    *   **Recursos Principais:** Mão de obra especializada (você) e software (o sistema a ser construído).
    *   **Estrutura de Custos:** Tempo e esforço dedicados.
2.  **Análise Estratégica:** Realize uma **Análise SWOT** (Forças, Fraquezas, Oportunidades e Ameaças) para o desenvolvimento do seu Mini-PMO Pessoal.
3.  **Termo de Abertura do Projeto (TAP):** Formalize o projeto, definindo o **Objetivo** e a **Justificativa**, as **Premissas** e **Restrições** (ex: o prazo é flexível; o recurso será apenas software local).
4.  **Partes Interessadas (Stakeholders):** Identifique as partes interessadas (o patrocinador, o gerente do projeto, o desenvolvedor, o cliente — todos sendo você, mas exigindo a compreensão do conceito).

### **Fase 2: Engenharia de Requisitos e Design** (Requisitos, DI e Qualidade)

É crucial definir o que o sistema deve fazer (requisitos funcionais) e como ele deve se comportar (requisitos não funcionais, especialmente usabilidade).

1.  **Requisitos Funcionais (RFs):** Defina os serviços que o sistema deve oferecer:
    *   RF1: Cadastrar, alterar e excluir Projetos e Tarefas.
    *   RF2: Associar Riscos a cada Tarefa.
    *   RF3: Calcular o **Caminho Crítico** de um conjunto de tarefas sequenciais.
2.  **Requisitos Não Funcionais (RNFs):**
    *   **Usabilidade:** O sistema deve ser **fácil de aprender, simples e usual**. O tempo de interação para operações corriqueiras deve ser minimizado (Modelo GOMS).
    *   **Segurança:** Acesso protegido (simulação de autenticação simples).
    *   **Qualidade (ISO/IEC 9126):** Definir o que garante a **Funcionalidade** e **Confiabilidade** do sistema.
3.  **Design de Interação (DI):** Esboce a interface (mesmo que seja de console) focando nos princípios de **Visibilidade** e **Bom Modelo Conceitual**. Assegure que as mensagens de erro (tratamento de exceções) sejam claras.
4.  **Matriz de Rastreabilidade:** Crie uma matriz ligando os principais requisitos (RFs e RNFs) aos objetivos do projeto e às entregas.

### **Fase 3: Modelagem, Estrutura e Lógica Matemática** (DB, Estrutura de Dados, Lógica)

Esta fase transforma os requisitos em modelos concretos, que servirão de planta para a implementação.

1.  **Modelagem de Dados (MER e Relacional):**
    *   Crie o **Diagrama Entidade-Relacionamento (DER)** para as entidades (ex: Projeto, Tarefa, Risco) e seus atributos.
    *   Defina as **Tuplas** (linhas) e **Atributos** (colunas) para o modelo relacional (base para o banco de dados).
    *   Defina operações de **restrição, projeção e união** (Álgebra Relacional) para consultas específicas.
2.  **Estrutura Analítica do Projeto (EAP):** Crie a EAP para o desenvolvimento do próprio software (e.g., Nível 1: Mini-PMO; Nível 2: Modelagem, Codificação, Testes; Nível 3: Pacotes de Trabalho).
3.  **Modelagem de Processo (BPMN):** Modele um processo-chave, como o fluxo de "Cálculo e Mitigação de Risco", utilizando notação **BPMN** (Eventos, Gateways, Atividades/Tarefas).
4.  **Lógica para Tempo e Risco:**
    *   **Caminho Crítico (Diagrama PERT):** Simule a aplicação do diagrama PERT a uma sequência de tarefas para determinar o tempo mínimo de conclusão do projeto.
    *   **Análise de Risco (Probabilidade):** Implemente a lógica de cálculo de risco, onde: $Risco = Probabilidade \times Impacto$. Utilize a **probabilidade** (Matemática para Computação) para ponderar o impacto de um risco, ajudando a priorizá-lo (Análise Qualitativa de Risco).

### **Fase 4: Algoritmos e Programação Orientada a Objetos (POO)**

Aqui você transforma os modelos em código, aplicando os conceitos de Algoritmos, Lógica de Programação e POO.

1.  **Estruturas Fundamentais:** Implemente a lógica em pseudocódigo (ou código real):
    *   Use comandos de **entrada (leia)**, **atribuição ($\leftarrow$)** e **saída (escreva)**.
    *   Aplique estruturas **condicionais (se-então/Caso)** (e.g., para classificar um risco como "alto" ou "baixo").
    *   Use estruturas de **repetição** (enquanto) para iterar sobre as listas de tarefas.
2.  **POO e Encapsulamento:**
    *   Crie as classes `Tarefa`, `Projeto`, `Risco`. Use **Encapsulamento** para proteger os atributos (dados).
    *   Aplique **Herança** (e.g., uma classe abstrata `Recurso` ou `EntidadeBase` que é herdada por `Tarefa` e `Risco`).
    *   Use **Polimorfismo** e **Sobrecarga** (e.g., um método `exibirDetalhes()` que se comporta de maneira diferente para Tarefa e Risco).
    *   Implemente o tratamento de **Exceções** (e.g., se o usuário tentar inserir uma data inválida ou um risco sem probabilidade).
3.  **Estrutura de Dados:**
    *   Utilize **estruturas heterogêneas (registros)** para armazenar informações de diferentes tipos (e.g., descrição em texto e prazo em data).
    *   Utilize **Listas Dinâmicas** para gerenciar as coleções de Tarefas ou Riscos.
    *   Otimize a busca por uma Tarefa concluída específica utilizando a lógica da **Busca Binária** (assumindo que as tarefas estão ordenadas por ID ou data de conclusão).

### **Fase 5: Infraestrutura e Sustentação** (SO, Redes, G.P. - Controle)

1.  **Arquitetura e SO:** Defina a aplicação como **Cliente/Servidor** (simples, de uma camada, onde o cliente acessa o banco de dados localmente). Considere os desafios de desempenho e o papel dos **threads** se processos concorrentes fossem adicionados (simulação mental).
2.  **Banco de Dados (SQL):** Use SQL para implementar as operações CRUD (Criação, Leitura, Atualização, Exclusão) no banco de dados.

| Operação | Conceitos de BD e SQL |
| :--- | :--- |
| Criar/Alterar Dados | Inserção/Atualização no Modelo Relacional. |
| Leitura/Busca Eficiente | Utilização de **índices** para consultas mais rápidas. |
| Relatórios | Consultas mais elaboradas da SQL envolvendo **funções de agregação**. |

3.  **Gerenciamento de Riscos e Qualidade (Controle):**
    *   Defina **Medidas de Desempenho** e **Custo** para monitorar o projeto (simulando, por exemplo, o Índice de Desempenho para o Término - IDPT).
    *   Crie um pequeno **Plano de Resposta a Riscos** (e.g., Estratégias de Mitigar, Transferir ou Aceitar).

---

### **Justificativa de Complexidade e Execução Solo**

O projeto é **complexo em conteúdo** porque:

*   Requer a modelagem matemática de Caminho Crítico (Lógica/G.P.).
*   Aplica conceitos de POO (Herança, Polimorfismo, Exceções).
*   Força a consideração de Design de Interação e Requisitos Não Funcionais (Usabilidade, Modelo GOMS).
*   Exige a integração de modelos de negócio (Canvas) com modelos de engenharia (DER, EAP, BPMN).

O projeto é **simples de realizar e pode ser feito sozinho** porque:

*   Não exige infraestrutura de rede complexa (pode ser um projeto local/console).
*   O banco de dados pode ser um arquivo local (como SQLite, evitando SGBDs complexos).
*   O foco está na aplicação *conceitual* (como estruturar as classes, como modelar o fluxo de dados, como escrever o algoritmo), em vez da escalabilidade ou performance industrial.

A prática e as atividades de autoestudo são essenciais para fixar todos esses conceitos.
