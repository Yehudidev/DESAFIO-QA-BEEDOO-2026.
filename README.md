# DESAFIO-QA-BEEDOO-2026

## Fluxo: Cadastro de Curso

### 001 - CursoCadastrar | Validação do campo "Número de Vagas"

**Background**  
Dado que o usuário acessou a tela **CursoCadastrar**

**Cenário**  
Usuário informa número de vagas negativo e o sistema aceita o cadastro.

- **Dado** que o usuário está na tela de cadastro de cursos  
- **Quando** o usuário preenche o campo **"Número de Vagas"** com um valor negativo  
- **E** envia o formulário de cadastro do curso  
- **Então** o sistema aceita o formulário  
- **E** o usuário é direcionado para a tela de cursos cadastrados  

**Evidência do Bug:**  
[Evidência do Bug](https://drive.google.com/file/d/1bMdvcsUlCytyCoP_BcRoW1-k19hdi8ZY/view?usp=drive_link)

**Severidade:** Média

---

### 002 - CursoCadastrar | Validação dos dados do curso

**Background**  
Dado que o usuário acessou a tela **CursoCadastrar**

**Cenário**  
O usuário informa dados incompatíveis e o sistema aceita o cadastro.

- **Dado** que o usuário está na tela de cadastro de cursos  
- **Quando** o usuário preenche a data de início com uma data no futuro  
- **E** preenche a data de término com uma data no passado  
- **E** envia o formulário de cadastro do curso  
- **Então** o sistema aceita o formulário  
- **E** o usuário é direcionado para a tela de cursos cadastrados  

**Evidência do Bug:**  
[Evidência do Bug](https://drive.google.com/file/d/1bMdvcsUlCytyCoP_BcRoW1-k19hdi8ZY/view?usp=drive_link)

**Severidade:** Média

---

### 003 - CursoCadastrar | Validação de formato de e-mail

**Background**  
Dado que o usuário acessou a tela **CursoCadastrar**

**Cenário**  
Usuário informa e-mail em formato inválido e o sistema aceita o cadastro.

- **Dado** que o usuário está na tela de cadastro de cursos  
- **Quando** o usuário digita um e-mail incompatível com o formato padrão  
- **E** envia o formulário de cadastro do curso  
- **Então** o sistema aceita o formulário  
- **E** o usuário é direcionado para a tela de cursos cadastrados  

**Evidência do Bug:**  
[Evidência do Bug](https://drive.google.com/file/d/1rxnq61mWaqq86VpjBF1Dy9n7QFyY4lK8/view?usp=drive_link)

**Severidade:** Média

---

### 004 - CursoCadastrar | Validação de campos obrigatórios

**Background**  
Dado que o usuário acessou a tela **CursoCadastrar**

**Cenário**  
Usuário envia o formulário sem preencher nenhum campo.

- **Dado** que o usuário está na tela de cadastro de cursos  
- **Quando** o usuário não preenche nenhum campo do formulário  
- **E** envia o formulário de cadastro do curso  
- **Então** o sistema aceita o formulário  
- **E** o usuário é direcionado para a tela de cursos cadastrados  

**Evidência do Bug:**  
[Evidência do Bug](https://drive.google.com/file/d/1ZSZgull99AG68lM_4JdnC9o8eMSNbNNg/view?usp=drive_link)

**Severidade:** Alta

---

### 005 - CursoCadastrar | Validação de endereço para curso presencial

**Background**  
Dado que o usuário acessou a tela **CursoCadastrar**

**Cenário**  
Usuário seleciona curso presencial e informa um endereço inválido.

- **Dado** que o usuário está na tela de cadastro de cursos  
- **Quando** o usuário seleciona a opção de cadastrar um **curso presencial**  
- **E** informa um endereço que não corresponde a um endereço válido  
- **E** envia o formulário de cadastro do curso  
- **Então** o sistema aceita o formulário  
- **E** o usuário é direcionado para a tela de cursos cadastrados  

**Evidência do Bug:**  
[Evidência do Bug](https://drive.google.com/file/d/1L7VHyjOjDPurwxuW9juF5SaJok5B9pgj/view?usp=drive_link)

**Severidade:** Alta

---

# Fluxo: Lista de Cursos

### 006 - ListaDeCursos | Verificação de opção de edição de cursos

**Background**  
Dado que o usuário acessou a tela **ListaDeCursos**

**Cenário**  
Usuário não encontra opção para editar um curso cadastrado.

- **Dado** que o usuário está na tela da lista de cursos cadastrados  
- **Quando** o usuário procura uma opção para modificar um curso já cadastrado  
- **E** verifica as ações disponíveis na lista de cursos  
- **Então** o usuário identifica que **não existe opção de editar o curso**

**Evidência do Bug:**  
[Evidência do Bug](https://drive.google.com/file/d/1ENhsfBMg9rThBJ1QrZwm9xj1S-CLyTZj/view?usp=drive_link)

**Severidade para o usuário:** Média

---

### 007 - ListaDeCursos | Exclusão de curso cadastrado

**Background**  
Dado que o usuário acessou a tela **ListaDeCursos**

**Cenário**  
Usuário tenta excluir um curso, porém ele permanece listado mesmo após mensagem de sucesso.

- **Dado** que o usuário está na tela de lista de cursos cadastrados  
- **Quando** o usuário clica na opção de excluir um curso já cadastrado  
- **E** o sistema apresenta uma mensagem de sucesso da exclusão  
- **Então** o curso **permanece listado** na tela de cursos cadastrados  

**Evidência do Bug:**  
[Evidência do Bug](https://drive.google.com/file/d/18_TZPd1uDghU4mZnUxdMwdl83fjfZge4/view?usp=drive_link)

**Severidade para o usuário:** Crítico

---

### 008 - ListaDeCursos | Funcionamento do botão "Listar Cursos"

**Background**  
Dado que o usuário acessou a tela **ListaDeCursos**

**Cenário**  
Usuário clica no botão "Listar Cursos" e nenhuma ação ocorre.

- **Dado** que o usuário está na tela da lista de cursos  
- **Quando** o usuário clica no botão **"Listar Cursos"**  
- **E** aguarda o carregamento da listagem  
- **Então** nenhuma ação é realizada pelo sistema  
- **E** a lista de cursos não é atualizada ou exibida  

**Evidência do Bug:**  
[Evidência do Bug](https://drive.google.com/file/d/15IQN-2c-OtLTxssqOp2GMCD45FpS7PtN/view?usp=drive_link)

**Severidade para o usuário:** Baixa

---

# Principais Correções

### 006 - Ausência de edição de cursos

Este bug deve ser tratado com prioridade, pois impacta diretamente a experiência do usuário ao manipular cursos já cadastrados, impossibilitando alterações rápidas e correções de informações.

### 007 - Falha na exclusão de cursos

Este bug está relacionado ao problema identificado no **Bug 006**.  
Sem a possibilidade de edição, o usuário pode optar por excluir o curso e cadastrá-lo novamente. Entretanto, como a exclusão não funciona corretamente, o usuário fica impossibilitado de corrigir ou modificar suas ações.

---

# Observações Finais

De forma geral, o **MVP apresenta funcionamento satisfatório**. No entanto, foram identificadas algumas ressalvas relacionadas:

- Ao espelhamento das informações exibidas nas caixas de texto em relação ao banco de dados  
- À ausência de funcionalidades de modificação de dados pelo cliente

---

# Informações do Teste

**QA:** Yehudi Souza  
**Sistema Operacional:** Windows 11  
**Máquina Utilizada:** Notebook  

**Ferramenta de apoio:**  
ChatGPT 5.3 utilizado para adaptação e estruturação dos cenários em formato BDD.
