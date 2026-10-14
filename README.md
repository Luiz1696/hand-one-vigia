# Vigia do CRM Hand One

Robô que confere o CRM a cada 5 minutos (`/api/v1/health`: site, banco, Redis e WhatsApp).

- **Caiu** (2 tentativas seguidas falharam): abre um alerta em *Issues* e manda e-mail para o suporte.
- **Voltou**: fecha o alerta e manda e-mail avisando.
- Uma vez por mês grava `batimento.txt`, porque o GitHub desliga robôs de repositórios parados há 60 dias.

O GitHub às vezes atrasa a execução alguns minutos — é normal.
