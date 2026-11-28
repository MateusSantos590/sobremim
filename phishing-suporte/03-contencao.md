# 3. Contenção: bloqueio e redefinição

## Passos em ordem

Se o usuário digitou credenciais, aja rápido: cada minuto é tempo de uso pelo atacante.

1. Encerre todas as sessões ativas da conta (revogar sessões no portal de administração).
2. Redefina a senha para uma temporária forte, com troca obrigatória no próximo login. Entregue por canal seguro (telefone ou pessoalmente), nunca por e-mail.
3. Revogue tokens e aplicativos conectados, para que o atacante não continue com acesso persistente.
4. Revise o MFA: remova métodos que o usuário não reconhece e registre os dele de novo.
5. Procure e apague regras de caixa suspeitas (encaminhamento externo, mover para pasta oculta, apagar respostas).
6. Bloqueie o domínio e a URL do phishing no gateway de e-mail e no proxy.
7. Pesquise o mesmo remetente e assunto nas outras caixas e remova as mensagens, se a ferramenta permitir.
8. Registre cada ação com horário no ticket.

Se o usuário só recebeu o e-mail e não interagiu: remova a mensagem, bloqueie o remetente e registre.

## Antes de reativar a conta

- Senha nova definida pelo usuário e MFA conferido.
- Nenhuma regra de caixa suspeita restante.
- Nenhum login ativo de IP desconhecido.
- Usuário orientado (ver seção 5).
- Segurança avisada, se algum gatilho do documento 4 se aplicar.

## O que o Suporte não faz sozinho

- Análise forense do dispositivo ou da caixa de correio.
- Bloqueios de rede em nível de firewall.
- Comunicação com clientes, órgãos ou autoridades sobre vazamento.
- Alteração de política de segurança.

Esses itens ficam com a Segurança da Informação.
