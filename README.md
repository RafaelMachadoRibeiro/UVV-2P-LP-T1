# Descrição do Sistema - Cadastro de Pessoas

O sistema desenvolvido em Python tem como objetivo gerenciar o cadastro de pessoas, permitindo que o usuário realize operações como adicionar, listar, consultar e remover cadastros, com a persistência dos dados sendo feita por meio de um arquivo CSV.

## Funcionalidades

1. **Cadastro de Pessoas**:
   - O sistema permite que o usuário cadastre novas pessoas inserindo informações como nome e idade. Cada cadastro recebe um identificador único (ID) gerado automaticamente pelo sistema de forma sequencial, garantindo que cada pessoa cadastrada tenha um número de identificação exclusivo.

2. **Listagem de Cadastros**:
   - O sistema oferece uma funcionalidade que exibe todos os cadastros registrados, listando o ID, nome e idade de cada pessoa cadastrada. Isso possibilita ao usuário visualizar rapidamente todos os dados armazenados no sistema.

3. **Consulta de Cadastros**:
   - Com a operação de consulta, o usuário pode buscar um cadastro específico pelo ID, permitindo a visualização dos detalhes da pessoa registrada com aquele identificador.

4. **Remoção de Cadastros**:
   - O sistema permite a remoção de cadastros, bastando o usuário informar o ID da pessoa que deseja excluir. O sistema então remove o registro correspondente, atualizando a lista de cadastros e o arquivo CSV de forma automática.

5. **Persistência de Dados**:
   - Todas as operações de cadastro, consulta, listagem e remoção são realizadas sobre uma lista de dicionários em memória, mas os dados são mantidos de forma persistente em um arquivo CSV. Ao iniciar o sistema, os cadastros são carregados do CSV, e ao final de cada execução, todas as alterações são salvas no arquivo, garantindo que o usuário possa continuar de onde parou em execuções futuras.

## Arquivo CSV

O arquivo CSV gerado pelo sistema contém três colunas: `ID`, `Nome`, e `Idade`. A primeira linha do arquivo CSV corresponde aos cabeçalhos, e as linhas subsequentes armazenam as informações dos cadastros realizados.

Durante a execução do sistema, foram realizadas as seguintes operações para gerar o arquivo CSV:

1. Foram criados os seguintes três usuários iniciais: **Rafael**, **Wagner** e **Luan**, que foram registrados no sistema com IDs 1, 2 e 3, respectivamente.
2. Após a criação, os cadastros foram listados, possibilitando visualizar o ID associado a cada pessoa.
3. O usuário **Luan**, de ID 3, foi removido do sistema utilizando a funcionalidade de exclusão.
4. Em seguida, foram cadastrados dois novos usuários: **Matheus** e **Abrantes**, que receberam os IDs 4 e 5, mantendo a continuidade da numeração de identificadores.

Essas operações demonstram que o sistema gerencia corretamente a criação, exclusão e atualização de cadastros, além de garantir a persistência dos dados no arquivo CSV.
