# TOME Líder

**Único APK que envia relatórios ao PCP e à Qualidade**  
TOME S/A — Usinagem

[![Android](https://img.shields.io/badge/Android-APK-3DDC84?logo=android&logoColor=white)](./Tome_Lider.apk)
[![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?logo=flutter&logoColor=white)](https://flutter.dev)

| | |
|---|---|
| **APK** | [`Tome_Lider.apk`](./Tome_Lider.apk) |
| **Pacote** | `com.tome.lider` |
| **Irmão** | [APK-PRODUCAO](https://github.com/ALN2025/APK-PRODUCAO) |

---

## Fluxo

```
Operadores → enviam Diário / R-022 / Folha OF ao LÍDER
                    │
                    ▼
              APK Líder (este)
                    │
        ┌───────────┴───────────┐
        ▼                       ▼
   Relatório PCP          Relatório Qualidade
   (WhatsApp/Email…)      (R-022 e/ou Folha OF)
```

| Botão | Origem | Destino |
|-------|--------|---------|
| **Enviar PCP** | Diários importados | **PCP** |
| **Enviar R-022** | R-022 importados | **Qualidade** |
| Folha OF | importada | **Qualidade** (separado) |

---

## Abas

- **Importar** — recebe dos operadores  
- **Dados** — gera e **envia** PCP / Qualidade  
- **Códigos** — só consulta de legendas  

---

## Stack

Flutter · SQLite · excel · pdf · share_plus · flavor `lider`

---

## Assinatura

<p align="center"><img src="aln.png" alt="Dev A.L.N" height="48"/></p>
<p align="center"><b>Dev A.L.N</b> · TOME S/A · 2026</p>
