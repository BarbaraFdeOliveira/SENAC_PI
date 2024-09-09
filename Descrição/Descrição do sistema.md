# Descrição do Protótipo de Interface do Sistema

Este documento tem como objetivo apresentar uma breve descrição das telas do protótipo da interface do sistema desenvolvido por nossa equipe. Ele serve para descrever cada tela, suas funcionalidades e recursos, podendo também ser utilizado como um manual para o usuário.

Vamos começar pela primeira tela, a tela de login.

## Tela de Login

A tela de login segue o padrão já encontrado no mercado. Como teremos dois tipos de usuários na área logada, Pessoa Física (que possui CPF) e Pessoa Jurídica (que possui CNPJ), também há a opção para quem não é cadastrado realizar o respectivo cadastro.

![Login](https://github.com/user-attachments/assets/742bd9af-6873-48d8-a0fa-29861389ac6b)

Mas, como você pode se cadastrar caso ainda não tenha um registro? Você é:

- **Aluno?**
- **Professor?**
- **Fornecedor?**

A seguir, explicaremos como efetuar seu cadastro, dependendo da sua natureza, por meio das telas de cadastro.

## Cadastro Pessoa Física (Aluno ou Professor)

A tela de cadastro para Pessoa Física é simples e intuitiva. O usuário precisará preencher dados pessoais como CPF, nome, data de nascimento, e-mail, endereço e criar uma senha.

![Cadastro 01](https://github.com/user-attachments/assets/9c35cad7-b5aa-40a5-90e6-fa6923ad98b0)

Essa tela serve tanto para professores quanto para alunos. No entanto, o professor terá uma segunda tela para preencher. Falaremos sobre isso a seguir.

## Cadastro de Fornecedor

Se você for fornecedor, esta tela foi desenvolvida para você! Os dados solicitados são diferentes do cadastro de Pessoa Física, pois o fornecedor deve possuir uma pessoa jurídica com CNPJ próprio e nome fantasia, por exemplo.

![Cadastro forn](https://github.com/user-attachments/assets/5d6c059d-7473-472a-b9bf-41deee2b6a07)

Você preencherá os dados conforme o solicitado na tela e criará uma senha.

## Cadastro de Professor

Por fim, temos a segunda tela que o professor deve preencher. Nesta etapa, o professor adicionará informações que o diferenciam de um aluno, como a "disciplina de atuação" e se ele é contratado ou atua como pessoa jurídica, prestando serviços esporadicamente para a instituição de ensino. Caso seja pessoa jurídica, ele deve marcar a checkbox correspondente.

![Cadastro professor](https://github.com/user-attachments/assets/06cb4149-55ea-46b8-b2f1-eb074c6c3908)

---

# Funcionalidades Importantes

## Tela de Avaliação

Esta tela apresenta o desempenho do aluno nas matérias, mostrando todas as suas notas e a média. Ela pode ser acessada tanto pelo aluno quanto pelo professor.

![Avali](https://github.com/user-attachments/assets/a07c97e5-6c6f-4478-a58e-714ea2ccc724)

## Tela de Matrícula

Todos aqueles que desejam se tornar alunos precisam preencher seus dados na tela de matrícula. Entre esses dados, será necessário informar se a pessoa possui um fiador (gerente financeiro) e a forma de pagamento de sua preferência.

![Matr](https://github.com/user-attachments/assets/0531d441-d527-4058-8945-23260ecb654b)

## Tela de Delegar Notas

Essa tela permite que o professor registre as notas dos alunos. Primeiramente, ele seleciona a turma e o aluno, e por último, insere a nota correspondente.

![Delegar](https://github.com/user-attachments/assets/92f12d40-1b4e-4dec-8959-235c0f109d2a)

---

# Casos de Uso: Caminho Feliz e Caminho Triste

Vamos observar dois exemplos de casos de uso, abordando tanto o "caminho feliz" quanto o "caminho triste". Mas você sabe o que são esses termos e o que é um caso de uso?

## O que é um Caso de Uso?

Um caso de uso é a simulação de uma ação que o usuário realiza em uma determinada funcionalidade do sistema. Essa ação pode ter dois resultados:

1. **Sucesso (Caminho Feliz)**: O sistema deve fornecer ao usuário aquilo que ele solicita, desde que ele siga as regras do sistema. Chamaremos esse cenário de "caminho feliz".
2. **Insucesso (Caminho Triste)**: O sistema impede o usuário de realizar determinada ação porque ele não seguiu as diretrizes ou condições necessárias. Esse cenário será chamado de "caminho triste".

## Exemplos

### Tela de Login

**Caminho Feliz**  
**Cenário**: Usuário acessa a área logada com sucesso.

**Como usuário, eu:**
1. Acesso o site da instituição.
2. Digito meu e-mail de login corretamente.
3. Digito minha senha corretamente.
4. Clico em "Entrar".

**Resultado esperado**: Devo ser direcionado para a tela inicial.

**Caminho Triste**  
**Cenário**: Usuário tenta acessar a área logada, mas erra a senha.

**Como usuário, eu:**
1. Acesso o site da instituição.
2. Digito meu e-mail de login corretamente.
3. Digito minha senha incorretamente.
4. Clico em "Entrar".

**Resultado esperado**: Devo receber uma mensagem de erro e não ser direcionado para a tela inicial.

---

### Tela de Seleção de Material

**Caminho Feliz**  
**Cenário**: Usuário solicita material com sucesso.

**Como usuário, eu:**
1. Acesso a tela de Seleção de Material.
2. Digito meu nome no campo "Solicitante".
3. Digito o nome do material.
4. Seleciono o tipo de material.
5. Clico em "Consultar".

**Resultado esperado**: Devo verificar a disponibilidade dos materiais solicitados.

**Caminho Triste**  
**Cenário**: Usuário solicita material, mas esquece de selecionar o tipo de material.

**Como usuário, eu:**
1. Acesso a tela de Seleção de Material.
2. Digito meu nome no campo "Solicitante".
3. Digito o nome do material.
4. Não seleciono o tipo de material.
5. Clico em "Consultar".

**Resultado esperado**: Devo receber um alerta do sistema solicitando que eu preencha o campo "Tipo de Material".
