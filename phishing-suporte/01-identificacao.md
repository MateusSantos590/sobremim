# 1. Identificação do e-mail suspeito

## E-mail de exemplo (fictício)

```
De: Suporte TI Acme <ti-suporte@acme-exemp1o.com.br>
Para: carlos.lima@acme-exemplo.com.br
Assunto: URGENTE: sua senha expira hoje

Prezado usuario,

Sua senha do Microsoft 365 expira em 24 horas. Para evitar o bloqueio
da sua conta, revalide agora:

https://acme-login-microsoft.example/verificar

Equipe de TI
```

O domínio real é `acme-exemplo.com.br`. O remetente usa `acme-exemp1o` (o número 1 no lugar da letra l).

## Sinais a verificar

| Sinal | O que olhar | No exemplo |
|---|---|---|
| Domínio parecido | Troca de letras, números no lugar de letras, domínio novo | `exemp1o` em vez de `exemplo` |
| Nome x endereço | O nome exibido pode ser qualquer um; confira o endereço | "Suporte TI Acme" vindo de domínio estranho |
| Autenticação | Cabeçalho `Authentication-Results` com SPF, DKIM ou DMARC em `fail` | SPF `fail` |
| Urgência | Prazo curto, ameaça de bloqueio | "expira em 24 horas" |
| Link | Passar o mouse mostra o destino real, sem clicar | Domínio sem relação com a Microsoft nem com a Acme |
| Saudação | Genérica em vez do nome da pessoa | "Prezado usuario" |
| Texto | Acentos faltando, tom diferente do usual da TI | Sem acento em "usuario" |
| Pedido | Pede senha, código MFA ou pagamento | Pede revalidação de senha |

Um sinal isolado pode ser coincidência. Dois ou mais justificam tratar como suspeito.

## Checklist rápido para o atendente

1. O endereço do remetente pertence ao domínio da empresa, letra por letra?
2. O e-mail cria urgência ou ameaça?
3. O link leva a um domínio que a empresa usa?
4. O pedido envolve senha, código ou dados pessoais?
5. A TI costuma pedir isso por e-mail? (Normalmente não.)
6. O cabeçalho mostra falha de SPF, DKIM ou DMARC?
7. Outros usuários receberam a mesma mensagem?

Duas respostas ruins ou mais: trate como phishing e siga para a coleta de evidências.
