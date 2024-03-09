# Ponderada-Cypress

1. Cypress é uma ferramenta de teste de frontend construída para a web moderna. A ferramenta aborda pontos críticos que os desenvolvedores e engenheiros de controle costumavam enfrentar ao testar aplicativos modernos. Serve para realizar testes automatizados que são realizados no navegador de forma a simular a interação do usuário com uma aplicação Web.
   
2. O Cypress possui algumas vantagens, como, facilidade de uso facilidade de uso, pois é fácil de configurar e utilizar, testes automatizados e manuais, possibilita qualquer forma de e desvantagens também, como, suporte limitado de navegador, inicialmente tem foco no chrome e sem suporte nativo para Testes Multi-tabs: Não suporta nativamente a execução de testes que necessitam abrir múltiplas abas ou janelas.
   
3. A arquitetura do Cypress é única porque executa os testes no mesmo loop de execução que a aplicação. Diferentemente de outras ferramentas que operam controlando o navegador de fora, Cypress executa dentro do navegador. Isso permite um controle mais direto e comandos mais rápidos, além de habilitar o acesso ao DOM e às APIs do navegador diretamente.
   
4. Cypress usa seletores de elementos para identificar os elementos da página com os quais interagir. Esses seletores podem ser qualquer string de seletores CSS, como IDs (**`#id`**), classes (**`.class`**), atributos (**`[attribute=value]`**), etc. Cypress também suporta seletores personalizados e oferece comandos para trabalhar com eles de maneira eficiente, como **`cy.get()`**, para selecionar elementos.
   
5.  Comandos e asserções no Cypress:
    ◦ **Comandos:** São funções que realizam ações, como visitar uma página (**`cy.visit()`**), clicar em um elemento (**`cy.click()`**), digitar em um campo de entrada (**`cy.type()`**), etc. Eles são encadeáveis e executados em sequência.
    ◦ **Asserções:** Verificam se certas condições são verdadeiras dentro de um teste. Por exemplo, verificar se um elemento está visível (**`should('be.visible')`**), se contém um texto específico (**`should('contain', 'texto')`**), etc. As asserções ajudam a garantir que a aplicação está funcionando como esperado.
    
6. **Descrição das etapas de preparação de um teste de interface, execução e verificação no Cypress.**
    ◦ **Preparação:** Inicia com a definição dos cenários de teste e a configuração do ambiente de teste, incluindo quaisquer dados ou estados de aplicação necessários.
    ◦ **Execução:** O Cypress inicia o navegador, carrega a aplicação e executa os comandos de teste definidos, como navegação, cliques, e entradas de dados.
    ◦ **Verificação:** Após a execução dos comandos, as asserções são usadas para verificar se o estado da aplicação corresponde ao esperado, como a presença de determinados elementos ou conteúdos.

7. Como estruturar testes de forma eficiente no Cypress?
- Separe os Testes por Funcionalidade: Organize seus testes em arquivos distintos com base em páginas ou funcionalidades específicas da sua aplicação.
- Agrupe Testes Relacionados: Utilize describe para agrupar testes relacionados e it para testes individuais, ajudando na organização e leitura.
- Abstraia com Page Objects: Simplifique os testes e reduza a duplicação criando objetos que representam páginas ou componentes específicos.
- Centralize Dados de Teste: Mantenha dados de teste, como credenciais de login, em arquivos separados para facilitar o gerenciamento.
- Utilize Hooks para Preparação e Limpeza: Aproveite beforeEach e afterEach para configurar o ambiente de teste antes de cada teste e limpar após a execução.
- Faça Testes Idempotentes: Garanta que cada teste possa ser executado de forma independente, sem afetar outros testes.
- Mantenha a Legibilidade: Escreva testes claros e fáceis de entender, visando a manutenção e compreensão por outros desenvolvedores.
