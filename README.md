# Proposta-de-Sistema-Orientado-a-Objetos-Segunda-Entrega

# Documentação do Sistema - Protótipos de Interface

## Introdução

Este repositório contém os protótipos de interface para diferentes jornadas do sistema, focados no cadastro de diversas entidades, incluindo Pessoa Física, Pessoa Jurídica, Professores, Fornecedores e Alunos.

## Jornadas de Cadastro

### 1. Cadastro de Pessoa Física

**Objetivo:** Permitir o cadastro eficiente e preciso de informações relacionadas a pessoas físicas no sistema.

**Principais Elementos de Interface:**
- Campos para CPF e email (login).
- Campo de senha (login).
- Botão para realizar cadastro ("Nâo possuo cadastro").
- Validação de dados para garantir a precisão das informações inseridas.
- Botão de confirmação para submissão do login.

**Fluxo de Interatividade:**
1. O usuário acessa a página de login/cadastro de Pessoa Física.
2. Preenche os campos obrigatórios no formulário.
3. Realiza a validação dos dados.
4. Submete o formulário para conclusão do login/cadastro.
5. Caso o período de matricula não estiver aberto o usuário vai ver uma tela informando a situação.
6. Caso haja disciplinas disponíveis serão mostradas na tela e a opção "matricular".
7. Tela de confirmar matrícula com todas as disciplinas selecionadas.
8. Caso alguma disciplona não tenha mais vaga isso será informado.
9. Matrícula realizada.

### 2. Cadastro de Pessoa Jurídica

**Objetivo:** Facilitar o registro de informações relacionadas a pessoas jurídicas no sistema.

**Principais Elementos de Interface:**
- Formulário específico para Pessoa Jurídica, incluindo campos para CPF e email.
- Campo de senha (login).
- Botão para realizar cadastro ("Nâo possuo cadastro").
- Validação de dados para garantir a precisão das informações inseridas.
- Botão de confirmação para submissão do login.

**Fluxo de Interatividade:**
1. O usuário acessa a página de  login/cadastro de Pessoa Jurídica.
2. Preenche os campos obrigatórios no formulário.
3. Realiza a verificação dos dados inseridos.
4. Submete o formulário para concluir o  login/cadastro.
5. Tela de detalhamento de solicitações pendentes de revisão.
6. Ao selecionar solicitação, tela com detalhamento da propsta.
7. Tela de solicitação aprovada/rejeitada.

## Caso de Uso: Matrícula em Disciplinas

**Ator:** Aluno

**Objetivo:** O Aluno matricula-se em disciplinas para o semestre letivo.

**Cenário Principal:**
1. O Aluno acessa o sistema de gestão acadêmica.
2. O Aluno insere seu login e senha.
3. O Aluno seleciona a opção "Matrícula".
4. O Aluno seleciona as disciplinas que deseja cursar.
5. O Aluno confirma a matrícula.
6. O sistema de gestão acadêmica processa a matrícula.

**Cenário Alternativo 1: Aluno não possui pré-requisitos:**
- O Aluno não possui as pré-requisitos para cursar uma disciplina: O sistema de gestão acadêmica exibe uma mensagem de erro e o Aluno deve consultar o currículo acadêmico.

**Cenário Alternativo 2: Não há vaga para a disciplina solicitada:**
- As vagas para uma disciplina estão preenchidas: O sistema de gestão acadêmica exibe uma mensagem de erro e o Aluno deve selecionar outra disciplina.

**Pré-condição:**
- O Aluno deve estar matriculado na instituição.

**Pós-condição:**
- O Aluno está matriculado nas disciplinas selecionadas.

## Caso de Uso: Consultar Notas, Avisos e Materiais

**Objetivo:** O Aluno consulta as notas, avisos e materiais das disciplinas que está cursando.

**Cenário Principal:**
1. O Aluno acessa o sistema de gestão acadêmica.
2. O Aluno insere seu login e senha.
3. O Aluno seleciona a opção "Consulta".
4. O Aluno seleciona a disciplina que deseja consultar.
5. O sistema de gestão acadêmica exibe as notas, avisos e materiais da disciplina selecionada.

**Cenário Alternativo 1: Aluno não está matriculado na disciplina:**
- O Aluno não está matriculado na disciplina selecionada: O sistema de gestão acadêmica exibe uma mensagem de erro e o Aluno deve selecionar outra disciplina.

**Cenário Alternativo 2: Informações não disponíveis:**
- Caso algum campo obrigatório não seja preenchido, o sistema exibe uma mensagem de erro e solicita que a informação seja preenchida.

**Pré-condição:**
- O Aluno deve estar matriculado na instituição.

**Pós-condição:**
- O Aluno está ciente das notas, avisos e materiais das disciplinas que está cursando.

## Caso de Uso: Preparar e Compartilhar Material Didático

**Ator:** Professor

**Objetivo:** O Professor prepara e compartilha material didático com os alunos.

**Cenário Principal:**
1. O Professor acessa o sistema de gestão acadêmica.
2. O Professor insere seu login e senha.
3. O Professor seleciona a opção "Material Didático".
4. O Professor cria ou edita o material didático.
5. O Professor publica o material didático.
6. Os alunos podem acessar o material didático.

**Cenário Alternativo 1: Material inválido:**
- O material didático é inválido ou inadequado: O sistema de gestão acadêmica exibe uma mensagem de erro e o Professor deve corrigir o material didático.

**Cenário Alternativo 2: Informações não disponíveis:**
- Caso algum campo obrigatório não seja preenchido, o sistema exibe uma mensagem de erro e solicita que a informação seja preenchida.

**Pré-condição:**
- O Professor deve ser credenciado pela instituição.

**Pós-condição:**
- O material didático está disponível para os alunos.

## Caso de Uso: Registro de Fornecimento de Produtos e Serviços

**Ator:** Fornecedor

**Objetivo:** O Fornecedor registra o fornecimento de produtos e serviços à instituição.

**Cenário Principal:**
1. O Fornecedor acessa o sistema de gestão acadêmica.
2. O Fornecedor insere seu login e senha.
3. O Fornecedor seleciona a opção "Fornecimento".
4. O Fornecedor registra os produtos e serviços fornecidos.
5. O sistema de gestão acadêmica processa o registro.

**Cenário Alternativo 1: Informações incorretas:**
- As informações fornecidas pelo Fornecedor são incorretas ou incompletas: O sistema de gestão acadêmica exibe uma mensagem de erro e o Fornecedor deve corrigir as informações.

**Cenário Alternativo 2: Informações já cadastradas:**
- Caso o fornecedor já tenha cadastrado informações no sistema, o sistema exibe uma mensagem informando que o fornecedor já cadastrou o fornecimento de produto ou serviço naquele período e exibe mensagem questionando se deseja repetir a informação.

**Pré-condição:**
- O Fornecedor deve ser credenciado pela instituição.

**Pós-condição:**
- O fornecimento de produtos e serviços é registrado.

## Conclusão

Os protótipos de interface fornecem uma representação visual das jornadas de cadastro no sistema, visando garantir uma experiência de usuário intuitiva e eficiente. A implementação destes protótipos facilitará o desenvolvimento e uso do sistema, promovendo a eficácia nas operações de cadastro.
