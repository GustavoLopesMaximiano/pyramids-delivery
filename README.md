# Pyramids delivery 
*Pyramids delivery*

Nosso site foi desenvolvido especialmente para apoiar transportadoras de pequeno porte, oferecendo soluções práticas e eficientes. Oferecemos três serviços principais: a organização e gestão das notas fiscais das entregas, a recomendação das rotas mais eficientes, e a possibilidade de rastrear as entregas em tempo real, garantindo mais controle e agilidade no processo logístico.

Equipe:
- [Adrio José de Oliveira](github.com/adriojose)
- [Emanuel Cipriano da Silva](github.com/Wtfemanu)
- [Gustavo Lopes Maximiano](github.com/gustavolopesmaximiano)
- [Matheus da Maia](github.com/matheusdamaia)
- [Thiago Gabriel Gonçalves do Nascimento](github.com/ThiagoGabrielNascimento)
- [Willian Marcelo Nobre](github.com/Williannobre)

Links do projeto:
-   Backend: [Repositório](https://github.com/GustavoLopesMaximiano/pyramids-delivery-Back) e [Publicação]()
-   Frontend: [Repositório](github.com/marcoandre/pi-frontend) e [Publicação]()

*Descrição do projeto:*

O Pyramids Delivery é um sistema desenvolvido para auxiliar no gerenciamento de fretes de caminhão:
- A plataforma permite cadastrar cargas, motoristas, rotas
- acompanhar entregas, facilitando a organização logística e reduzindo erros operacionais.

*Situação problema:*

Atualmente, muitos transportadores e pequenos negócios ainda fazem o controle de fretes manualmente, utilizando papel ou planilhas simples. Isso gera problemas como:
- Falta de organização das entregas
- Dificuldade em planejar rotas eficientes
- Perda de informações importantes
- Atrasos nas entregas
- Dificuldade em calcular custos e lucros

*Descrição da proposta:*

O projeto propõe a criação de um sistema digital que:
- Permite cadastrar fretes (origem, destino, carga, valor)
- Organizar rotas de forma simples
- Registra motoristas e veículos
- Mostra o status das entregas (pendente, em andamento, entregue)
- Ajuda no controle financeiro básico
- O sistema sera desenvolvido como um site (PWA) acessível por celular e computador, facilitando o uso no dia a dia dos motoristas e gestores.

 *Requisitos Funcionais*
 
- RF001: O sistema deve permitir cadastro de novos usuários.
  - RN001.1: O email deve ser único no sistema.
  - RN001.2: A senha deve ter no mínimo 6 caracteres.
- RF002: O sistema deve permitir login com email e senha.
  - RN002.1: O login só deve ser permitido com credenciais válidas.
- RF003: O sistema deve permitir logout do usuário.
- RF004: O sistema deve exibir um resumo de fretes.
- RF005: O sistema deve mostrar status das entregas (pendente, em andamento, entregue).
  - RN005.1: Os status devem seguir o padrão: Pendente → Em andamento → Entregue.
- RF006: O sistema deve fornecer acesso rápido aos módulos principais.
- RF007: O sistema deve permitir cadastrar cargas.
  - RN007.1: A carga deve possuir descrição, peso e valor obrigatórios.
- RF008: O sistema deve permitir editar cargas.
- RF009: O sistema deve permitir excluir cargas.
  - RN009.1: Não é permitido excluir cargas vinculadas a fretes.
- RF010: O sistema deve armazenar descrição, peso e valor da carga.
  - RN10.1: O peso e valor devem ser maiores que zero.
- RF011: O sistema deve permitir cadastrar motoristas.
  - RN011.1: O motorista deve possuir nome e CNH obrigatórios.
- RF012: O sistema deve permitir editar motoristas.
- RF013: O sistema deve permitir excluir motoristas.
  - RN013.1: Não é permitido excluir motoristas vinculados a fretes ativos.
- RF014: O sistema deve armazenar nome e CNH.
- RF015: O sistema deve permitir cadastrar veículos.
  - RN015.1: A placa do veículo deve ser única.
- RF016: O sistema deve permitir editar veículos.
- RF017: O sistema deve permitir excluir veículos.
  - RN017.1: Não é permitido excluir veículos vinculados a fretes ativos.
- RF018: O sistema deve armazenar placa, modelo e capacidade.
  - RN018.1: A capacidade deve ser maior que zero.
- RF019: O sistema deve permitir cadastrar rotas.
  - RN19.1: A rota deve conter ponto inicial e final obrigatórios.
- RF020: O sistema deve permitir editar rotas.
- RF021: O sistema deve permitir excluir rotas.
  - RN021.1: Não é permitido excluir rotas vinculadas a fretes.
- RF022: O sistema deve armazenar ponto inicial, ponto final e distância.
  - RN22.1: A distância deve ser maior que zero.
- RF023: O sistema deve permitir criar fretes.
  - RN023.1: Todos os dados obrigatórios devem ser informados.
- RF024: O sistema deve associar carga, motorista, veículo e rota ao frete.
  - RN024.1: Todos os itens devem estar previamente cadastrados.
- RF025: O sistema deve permitir definir origem e destino.
  - RN025.1: Origem e destino são obrigatórios.
- RF026: O sistema deve permitir informar valor do frete.
  - RN026.1: O valor do frete deve ser maior que zero.
- RF027: O sistema deve definir automaticamente o status inicial como "Pendente".
  - RN027.1: O status inicial deve ser sempre "Pendente".
- RF028: O sistema deve criar automaticamente uma entrega ao criar um frete.
  - RN028.1: Toda entrega deve estar vinculada a um frete.
- RF029: O sistema deve permitir atualização de status da entrega.
  - RN029.1: Não é permitido pular etapas do status.
- RF030: O sistema deve permitir registrar data de entrega.
  - RN030.1: A data só pode ser registrada quando o status for "Entregue".
- RF031: O sistema deve permitir adicionar observações.
- RF032: O sistema deve atualizar os dados do dashboard automaticamente.
- RF033: O sistema deve permitir atualização de status por motoristas/gestores.
- RF034: O sistema deve permitir visualizar histórico de fretes.
- RF035: O sistema deve permitir filtrar por status.
- RF036: O sistema deve permitir filtrar por data.
- RF037: O sistema deve exibir informações de custos e valores.
  - RN037.1: Apenas fretes finalizados devem compor os cálculos.
- RF038: O sistema deve permitir análise de desempenho das entregas.

*Requisitos Não Funcionais*

- RNF001: O sistema deve responder às ações do usuário em até 3 segundos.
  - RNF001.1: O tempo de resposta deve ser medido em operações principais (login, cadastro, criação de frete).
- RNF002: O dashboard deve atualizar em tempo real ou com atraso mínimo.
  - RNF002.1: As atualizações devem ocorrer automaticamente sem necessidade de recarregar a página.
- RNF003: O sistema deve criptografar senhas dos usuários.
  - RNF003.1: As senhas não devem ser armazenadas em texto puro.
- RNF004: O sistema deve garantir autenticação segura.
  - RNF004.1: O acesso deve exigir validação de credenciais antes de liberar funcionalidades.
- RNF005: O sistema deve proteger os dados contra acessos não autorizados.
  - RNF005.1: Apenas usuários autenticados podem acessar dados do sistema.
- RNF006: O sistema deve ser responsivo (funcionar em celular e desktop).
  - RNF006.1: A interface deve se adaptar a diferentes tamanhos de tela.
- RNF007: O sistema deve ter interface simples e intuitiva.
- RNF008: O sistema deve exigir poucos passos para realizar ações.
- RNF009: O sistema deve estar disponível 24/7.
  - RNF009.1: O sistema deve minimizar períodos de indisponibilidade.
- RNF010: O sistema deve funcionar como PWA (Progressive Web App).
  - RNF010.1: O sistema deve permitir acesso via navegador sem instalação obrigatória.
- RNF011: O sistema deve evitar perda de dados.
  - RNF011.1: O sistema deve persistir os dados em banco de dados confiável.
- RNF012: O sistema deve manter histórico de alterações.
  - RNF012.1: Alterações relevantes devem ser registradas para consulta futura.
- RNF013: O sistema deve suportar crescimento de usuários e dados.
  - RNF013.1: O sistema deve manter desempenho mesmo com aumento de dados.

*Tabela MER*

<img width="757" height="579" alt="image" src="https://github.com/user-attachments/assets/4f0a9908-7ee8-4164-893f-f73999130b44" />
