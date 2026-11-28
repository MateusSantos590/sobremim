# 4. Quando escalar para a Segurança da Informação

## Gatilhos de escalonamento

Um gatilho basta.

- O usuário digitou credenciais ou código MFA na página falsa.
- Há login de IP ou país incomum, ou fora do horário do usuário.
- Existe regra de encaminhamento ou de ocultação criada sem o usuário saber.
- A conta é privilegiada (administrador, financeiro, diretoria).
- A conta enviou e-mails para muitos destinatários após o incidente.
- O e-mail trazia anexo executável ou macro, e o usuário abriu.
- Há suspeita de acesso a dados sensíveis ou pessoais.
- Vários usuários receberam e interagiram com a mesma campanha.

## Severidade e prazo

Os prazos abaixo são sugestões para este projeto e devem seguir a política da empresa.

| Severidade | Critério | Prazo de acionamento |
|---|---|---|
| Baixa | E-mail recebido, sem clique | Registrar no mesmo dia |
| Média | Clique sem credencial, ou credencial digitada sem uso indevido confirmado | Em até 1 hora |
| Alta | Uso indevido confirmado, conta privilegiada, anexo executado ou dados expostos | Imediato, por telefone e ticket |

## Informações a entregar na passagem

- Número do ticket e severidade.
- Usuário afetado, cargo e privilégios.
- Linha do tempo: recebimento, clique, relato, contenção.
- Ações já executadas.
- Local da pasta de evidências e hashes.
- Outros usuários possivelmente afetados.
- O que ainda está pendente.
