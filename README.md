# Meu Controle Financeiro — edição pessoal

Aplicação React para uso pessoal, com armazenamento local no navegador (localStorage). Não requer conta Supabase, login, servidor ou conexão para salvar dados.

## Requisitos
- Windows 10/11
- Node.js LTS (20 ou superior recomendado)
- Conexão à internet para instalar dependências; depois o aplicativo roda localmente no navegador.

## Instalação no Windows
1. Baixe e instale Node.js LTS: https://nodejs.org/
2. Feche e reabra o Prompt de Comando. Teste `node -v` e `npm -v`. Ambos devem exibir uma versão.
3. Extraia o ZIP. Abra a pasta `controle-financeiro-pessoal` que contém `package.json`.
4. Na barra de endereço do Explorador de Arquivos, digite `cmd` e pressione Enter.
5. Execute `npm install` e aguarde terminar.
6. Execute `npm run dev`.
7. Abra o endereço local mostrado pelo terminal, normalmente `http://localhost:5173/`. Mantenha o terminal aberto enquanto usa o aplicativo.
8. Para encerrar, volte ao terminal e pressione `Ctrl+C`.

## Recursos
- Painel com receitas, despesas, saldo de contas e orçamento mensal.
- Histórico de receitas/despesas com edição, exclusão, pesquisa, filtros e exportação CSV.
- Categorias e limites de orçamento.
- Contas/carteiras com saldo inicial e saldo calculado pelas movimentações.
- Metas financeiras com valor desejado, progresso e prazo.
- Relatórios mensais e gráficos.
- Importação de PDF de contracheque com conferência manual antes de registrar.
- Dízimo/contribuição opcional e percentual configurável.
- Backup JSON e restauração.

## Dados e privacidade
Os dados são guardados no `localStorage` do navegador deste dispositivo e perfil de usuário. Não há sincronização automática entre computadores/celulares. Se limpar os dados do navegador, pode perder seus registros. Use Configurações → Baixar backup completo com frequência. O backup contém dados financeiros e deve ser guardado em local privado.

A leitura do PDF pode falhar em documentos digitalizados como imagens, protegidos ou com texto em layout incomum. Confira sempre o valor e a data antes de registrar. O app não é aconselhamento financeiro nem sistema bancário.

## Gerar versão de produção
Execute `npm run build`. Os arquivos prontos serão criados na pasta `dist`.
