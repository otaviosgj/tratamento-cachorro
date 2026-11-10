# 🐾 Tratamento do Bebê — Acompanhamento de tratamento dermatológico

Aplicativo web simples (arquivo único, `index.html`) para acompanhar o tratamento de pele de um cachorro,
com checklist diário, calendário do tratamento, progresso por medicamento, timer do banho e lembretes por notificação.

## 💊 Tratamentos incluídos

| Tratamento | Frequência | Período |
|---|---|---|
| 👂 Otosyn (otológico) | 4 gotas em cada ouvido, a cada 12h | 14 dias |
| 🧻 Lenço Clorexidine 3% + D-Pantenol 1% | Passar no corpo, a cada 12h | 28 dias |
| 💊 SAME 54 mg (cápsula) | 1 a cada 24h | 30 dias |
| 🛁 Ketochlor Xampu | Banho a cada 3 dias (agir 10 min) | 6 semanas |

Dados de início: Otosyn 28/10 às 21h · Lenço 30/10 às 21h · SAME 31/10 às 21h · Xampu 04/11.

## ✨ Funcionalidades

- **Próximo cuidado** — cartão com o horário da próxima dose e contagem regressiva
- **Hoje** — checklist da manhã (09h) e da noite (21h), com botão ✔ para marcar cada dose
- **Timer de 10 minutos** para o tempo de ação do xampu no corpo
- **Calendário do tratamento** — dias verdes (completos), amarelos (pela metade) e vermelhos (não feitos);
  toque em um dia para ver e marcar as doses individualmente
- **Dias passados marcados automaticamente** — o acompanhamento começa a partir do dia atual
- **Bloqueio de dias passados** — após o dia terminar, os dados ficam somente para visualização
- **🔔 Notificações** — aviso no horário de cada dose (requer permitir notificações, com o app aberto)
- **Barras de progresso** por tratamento, com total de doses e data final
- Dados salvos no navegador (localStorage) — nada é enviado para servidores

## 📱 Como usar

1. Abra o `index.html` em qualquer navegador (celular ou computador), **ou** acesse a versão publicada no **GitHub Pages**
2. No celular, recomenda-se: Chrome → menu ⋮ → **"Adicionar à tela de início"** (vira um ícone como app)
3. Toque em **"Ativar"** para receber os lembretes no horário das doses

> 💡 Os dias anteriores a hoje já vêm marcados, pois o tratamento começou antes do app existir.

## 🛠️ Tecnologia

- HTML + CSS + JavaScript puros — sem dependências, sem build
- Emissão de datas calculada dinamicamente a partir das datas de início
- Estado persistido em `localStorage`
