# TOME Líder

**Recebimento e relatórios PCP / Qualidade**  
TOME S/A — Usinagem

[![Android](https://img.shields.io/badge/Android-APK-3DDC84?logo=android&logoColor=white)](./Tome_Lider.apk)
[![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?logo=flutter&logoColor=white)](https://flutter.dev)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

| | |
|---|---|
| **APK** | [`Tome_Lider.apk`](./Tome_Lider.apk) |
| **Pacote** | `com.tome.lider` |
| **Público** | Líder — importar e gerar relatórios |
| **Irmão** | [APK-PRODUCAO](https://github.com/ALN2025/APK-PRODUCAO) |
| **Atualização** | 04/08/2026 |

---

## O que o líder recebe

Do APK Produção (arquivos **separados**):

| Arquivo | Conteúdo | Relatório |
|---------|----------|-----------|
| **Diário** | Qtd produzida + paradas (Legendas) | **PCP** |
| **R-022** | Cotas críticas do dia | **Qualidade** (planilha diária) |
| **Folha OF** | Roteiro OF (quando o operador salvar) | **Qualidade** (não junta com R-022) |

Envio ao time: WhatsApp / Telegram / Email.

---

## Abas

| Aba | Função |
|-----|--------|
| **Importar** | Bluetooth / receber direto / XLS / PDF |
| **Dados** | Ver importado + gerar **PCP** e **R-022** (PDF/XLS) |
| **Códigos** | Só **consultar** legendas (parada, sucata, U/F, roteiro OF). Não é relatório |

---

## Fluxo

```mermaid
flowchart LR
  op[APK Produção]
  imp[Importar]
  dados[Dados]
  op -->|Diário| imp
  op -->|R-022| imp
  op -->|Folha OF| imp
  imp --> dados
  dados --> pcp[PCP]
  dados --> qual[Qualidade]
```

---

## Stack

| Camada | Tecnologia |
|--------|------------|
| UI | Flutter / Dart 3 |
| Banco | SQLite (`tome_lider.db`) |
| Import | `file_picker` + Excel/CSV |
| Export | `excel` + `pdf` |
| Share | `share_plus` |
| Flavor | `lider` (`com.tome.lider`) |

---

## Instalação

1. Desinstale a versão antiga.  
2. Instale [`Tome_Lider.apk`](./Tome_Lider.apk).  

---

## Compilar

```bash
flutter build apk --release --flavor lider --dart-define=FLAVOR=lider
```

---

## Assinatura

<p align="center">
  <img src="aln.png" alt="Dev A.L.N" height="48"/>
</p>

<p align="center"><b>Dev A.L.N</b> · TOME S/A · 2026</p>

- Produção: https://github.com/ALN2025/APK-PRODUCAO  
- Líder: https://github.com/ALN2025/APK-LIDER  
