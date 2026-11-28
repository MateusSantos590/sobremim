# 2. Evidências a coletar

Colete antes de remover qualquer coisa. Depois da limpeza, parte delas some.

## Lista de coleta

| Evidência | Onde obter | Por que importa |
|---|---|---|
| E-mail original em `.eml` | Anexar como mensagem, não encaminhar | Preserva cabeçalhos completos |
| Cabeçalhos (`Received`, `Return-Path`, `Authentication-Results`) | Dentro do `.eml` | Mostram a origem real e as falhas de SPF, DKIM e DMARC |
| URL do link | Copiar sem clicar | Permite bloquear e analisar o destino |
| Hash SHA-256 de anexos | `Get-FileHash arquivo` no PowerShell | Identifica o arquivo sem abri-lo |
| Horário do recebimento e do clique | Relato do usuário e log do gateway de e-mail | Define a janela de exposição |
| Logs de login | Portal de administração, relatório de entradas | IP, local e dispositivo de cada acesso, inclusive os que o usuário não reconhece |
| Regras de caixa | Configurações de regras do e-mail | Atacantes criam encaminhamentos e regras que ocultam respostas |
| Itens enviados | Pasta Enviados e rastreamento de mensagens | Mostra se a conta foi usada para novos ataques |
| Métodos de MFA registrados | Perfil de segurança do usuário | Detecta método adicionado pelo atacante |
| Capturas de tela | Página falsa, alertas, relato do usuário | Registro visual para o ticket |

## Como preservar

1. Salve tudo em uma pasta por incidente, nomeada `INC-AAAAMMDD-NN` (por exemplo, `INC-20261128-01`).
2. Nomeie os arquivos com data e tipo: `2026-11-28_email-original.eml`.
3. Gere o hash de cada arquivo e anote no ticket.
4. Restrinja o acesso à pasta ao Suporte e à Segurança.
5. Mantenha uma tabela simples de custódia: quem acessou, quando e por quê.
6. Não abra anexos nem links na máquina do usuário nem na sua. Se precisar analisar, use um ambiente isolado indicado pela Segurança.
