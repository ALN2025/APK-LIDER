<div align="center">

<img src="aln.png" alt="Dev A.L.N" height="72"/>

# TOME Líder

### Importar · PCP · Qualidade  
**TOME S/A · Usinagem**

[![APK](https://img.shields.io/badge/Download-Tome__Lider.apk-FF6D00?style=for-the-badge&logo=android&logoColor=white)](./Tome_Lider.apk)
[![Produção](https://img.shields.io/badge/Irmão-APK--PRODUCAO-00C853?style=for-the-badge&logo=github)](https://github.com/ALN2025/APK-PRODUCAO)
[![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)

`com.tome.lider` · celular do líder · **único que envia ao PCP**

</div>

---

## Por que este APK?

Os operadores mandam XLS/PDF para você.  
**Só o Líder** consolida e envia:

| Relatório | Origem | Você envia para |
|-----------|--------|-----------------|
| **PCP** | Diários importados | **PCP** |
| **Qualidade R-022** | R-022 do dia | **Qualidade** |
| **Folha OF** | Ordem (quando vier) | **Qualidade** (separado) |

WhatsApp · Telegram · Email — a partir do seu celular.

---

## Fluxo

```mermaid
flowchart LR
  OP1[Operador A]
  OP2[Operador B]
  IMP[Importar]
  DADOS[Aba Dados]
  PCP[PCP]
  QUAL[Qualidade]

  OP1 -->|Diário + R-022| IMP
  OP2 -->|Diário + R-022| IMP
  IMP --> DADOS
  DADOS -->|Enviar PCP| PCP
  DADOS -->|Enviar R-022 / OF| QUAL
```

```
  ┌─────────────┐     XLS/PDF      ┌──────────────┐
  │  Produção   │ ───────────────► │    LÍDER     │
  │  (vários)   │                  │  (este APK)  │
  └─────────────┘                  └──────┬───────┘
                                          │
                         ┌────────────────┼────────────────┐
                         ▼                                 ▼
                   Enviar PCP                        Enviar Qualidade
                   (WhatsApp…)                       (R-022 / Folha OF)
```

---

## Abas

| Aba | Função |
|-----|--------|
| **Importar** | Receber direto / Bluetooth / escolher arquivo |
| **Dados** | Ver produção · **Enviar PCP** · **Enviar R-022** |
| **Códigos** | Só **consultar** legendas (não é relatório) |

---

## Download

### [`Tome_Lider.apk`](./Tome_Lider.apk)

1. Desinstale a versão antiga  
2. Instale o APK  
3. Nome + Setor → Importar → Dados  

---

## Stack

| | |
|---|---|
| UI | Flutter / Dart 3 |
| Banco | SQLite (`tome_lider.db`) |
| Import | `file_picker` · Excel/CSV |
| Export | `excel` + `pdf` |
| Share | `share_plus` |
| Flavor | `lider` |

---

<div align="center">

<br/>

<img src="aln.png" alt="Dev A.L.N" height="56"/>

### Desenvolvido por **Dev A.L.N**

[github.com/ALN2025](https://github.com/ALN2025) · TOME S/A · 2026

</div>
