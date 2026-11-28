# 6. Registro do incidente

## Modelo de ticket

| Campo | Preenchimento |
|---|---|
| ID | INC-AAAAMMDD-NN |
| Data e hora do registro | |
| Reportante | |
| Usuário afetado | |
| Severidade | Baixa, média ou alta |
| Descrição | O que aconteceu, em poucas linhas |
| Evidências | Caminho da pasta e hashes |
| Ações executadas | Cada ação com horário |
| Escalonado para a Segurança | Sim ou não, com horário e responsável |
| Responsável | |
| Status | Aberto, em contenção, encerrado |
| Lições aprendidas | |

## Linha do tempo (cenário preenchido)

Todos os dados são fictícios.

| Horário | Evento | Ação |
|---|---|---|
| 08:42 | Carlos Lima recebe o e-mail falso | |
| 08:50 | Carlos clica no link e digita as credenciais | |
| 11:15 | Carlos nota e-mails enviados que não escreveu e abre chamado | Ticket INC-20261128-01 criado, severidade média |
| 11:20 | Suporte coleta o `.eml` e os logs de login | Evidências salvas e hashes registrados |
| 11:28 | Logs mostram login de IP desconhecido às 09:03 | Severidade elevada para alta |
| 11:30 | Sessões encerradas, senha redefinida, tokens revogados | Contenção executada |
| 11:36 | Encontrada regra que encaminha mensagens a endereço externo | Regra removida |
| 11:40 | Segurança acionada por telefone e ticket | Passagem com resumo e evidências |
| 11:55 | Domínio e URL bloqueados, e-mail removido de outras caixas | Busca em todas as caixas |
| 12:20 | Carlos orientado e MFA registrado de novo | Conta reativada |
| 12:30 | Comunicado de conscientização enviado à equipe | |

## Causa raiz e ações preventivas

Causa raiz: e-mail de phishing com domínio parecido chegou à caixa do usuário, e a conta não exigia MFA resistente a phishing.

| Ação | Responsável | Prazo |
|---|---|---|
| Ativar o botão "Reportar phishing" para todos | TI | 15 dias |
| Exigir MFA por aplicativo ou chave física nas contas do financeiro | Segurança | 30 dias |
| Alertar sobre domínios parecidos com o da empresa | Segurança | 30 dias |
| Treinar a equipe com simulação de phishing | Suporte e Segurança | 60 dias |
| Revisar este roteiro após o primeiro caso real | Suporte | Contínuo |
