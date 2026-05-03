# Fase 3 — Mês 4-6: Automação Total
**Tempo:** 30-45 min/dia · 60 dias

> Objetivo: o negócio roda sem você. Conteúdo agendado, funil convertendo, afiliados promovendo, entrega automática.

---

## O que Automatizar e Como

### Mapa de Automação Completo

```
ENTRADA DE TRÁFEGO (automático)
Pins agendados no Pinterest (30 dias à frente)
    +
Instagram Carrossel agendado (Buffer free ou Later free)
    ↓
CAPTURA DE LEADS (automático via Systeme.io)
Form → e-mail de boas-vindas → sequência de 5 e-mails
    ↓
VENDA (automático)
Sequência de e-mails → página de vendas → checkout Systeme.io
    ↓
ENTREGA (automático via Systeme.io)
Compra confirmada → link do produto enviado → acesso liberado
    ↓
PÓS-VENDA (automático)
E-mail de onboarding → upsell → recompra em 30 dias
    ↓
AFILIADOS (automático)
Outros criadores promovem → comissão calculada automaticamente
```

---

## Automações com Make.com (Plano Grátis — 1.000 ops/mês)

### Cenário 1: Alerta de Pin Viral

**O que faz:** quando um pin ultrapassa 500 saves, você recebe notificação no WhatsApp via CallMeBot (grátis).

**Módulos no Make.com:**
1. Pinterest → Watch Pins (verificar 1x por dia)
2. Filter: saves > 500
3. HTTP → CallMeBot API (enviar mensagem WhatsApp grátis)

**Por que é útil:** identificar qual conteúdo ressoa para criar variações imediatamente.

---

### Cenário 2: Tracking de Leads em Planilha

**O que faz:** cada novo lead no Systeme.io é adicionado automaticamente a uma planilha Google Sheets com data, fonte e e-mail.

**Módulos no Make.com:**
1. Webhook (Systeme.io envia dados ao receber novo lead)
2. Google Sheets → Add Row (data, e-mail, fonte, data)

**Configuração no Systeme.io:**
- Funnels → seu funil → Settings → Integrations → Webhook
- URL do webhook: copiar do Make.com

---

### Cenário 3: Relatório Semanal Automático

**O que faz:** toda segunda-feira às 8h, você recebe um e-mail resumindo: leads da semana, vendas, e-mail com maior abertura.

**Módulos no Make.com:**
1. Schedule (toda segunda, 8h)
2. Google Sheets → Search Rows (filtrar pela semana anterior)
3. Gmail → Send Email (com resumo formatado)

---

### Cenário 4: Backup de Conteúdo

**O que faz:** quando você adiciona um arquivo PNG na pasta "Pinterest Pins" do Google Drive, ele é automaticamente registrado na planilha de controle de conteúdo.

**Módulos no Make.com:**
1. Google Drive → Watch Files in Folder
2. Google Sheets → Add Row (nome, data, status: "aguardando publicação")

---

## Automação de Conteúdo (sem Make.com)

### Agendamento de Pins (nativo do Pinterest — grátis)

1. Pinterest → criar pin → ao publicar, escolher "Agendar"
2. Agendar 30 dias de conteúdo de uma vez (2h a cada 30 dias)
3. Frequência recomendada: 3-5 pins por dia em horários variados

**Como criar 30 dias de pins em 2 horas:**
1. Abrir ChatGPT e pedir 60 ideias de título de pin (30 min)
2. No Canva, criar template base → duplicar 60 vezes e trocar apenas o texto (1h)
3. Baixar todos como ZIP → subir no Pinterest e agendar (30 min)

### Agendamento no Instagram

**Buffer free:** até 3 canais, 10 posts agendados por canal
1. Criar conta em buffer.com (grátis)
2. Conectar Instagram Business
3. Agendar 4 carrosséis por semana (1 mês = 16 posts, feitos em 2h)

---

## Programa de Afiliados do Seu Produto

Quando você tem afiliados, outras pessoas promovem seu produto gratuitamente e você paga só quando vende.

### Configurar no Systeme.io (grátis no plano free)

1. Systeme.io → Products → seu produto → Affiliates
2. Ativar programa de afiliados
3. Definir comissão: 40-50% (ex: produto R$47 → afiliado ganha R$18,80-R$23,50)
4. Criar página de cadastro de afiliados (Systeme.io gera automaticamente)
5. Link de afiliado: cada afiliado recebe link único rastreável

### Como recrutar afiliados (sem gastar nada)

- Postar no Pinterest/Instagram: "Afilie-se e ganhe 40% por venda. Link na bio."
- Enviar e-mail para sua lista: "Quer ganhar comissão promovendo este produto?"
- Grupos de WhatsApp/Telegram de marketing digital: anunciar o programa
- Outros criadores do nicho: oferecer produto grátis em troca de promoção

**Meta:** 10 afiliados ativos. Se cada um fizer 2 vendas/mês → 20 vendas extras sem trabalho.

---

## Rotina da Fase 3 (30-45 min/dia)

| Dia | Atividade | Tempo |
|---|---|---|
| Segunda | Checar relatório semanal automático + ajustar se necessário | 15 min |
| Terça | Criar batch de 60 pins (1x ao mês, 2h) | 2h (mensal) |
| Quarta-Sexta | Responder e-mails de clientes/afiliados | 15 min |
| Sábado | Revisar métricas do funil + otimizar 1 elemento | 30 min |
| Domingo | Checar comissões de afiliado + planilha de leads | 15 min |

**Total: ~3-4h por semana.**

---

## Métricas de Sucesso da Fase 3

| Métrica | Meta |
|---|---|
| Leads mensais | 300+ |
| Receita mensal | R$3.000-R$10.000 |
| Afiliados ativos | 10+ |
| Tempo dedicado/dia | < 45 min |
| Vendas via afiliados | > 30% do total |

**Ao concluir esta fase → acesse [`../fase-4/piloto-automatico.md`](../fase-4/piloto-automatico.md)**
