<div align="center">

<img src="aln.png" alt="Dev A.L.N" height="72"/>

# TOME Líder

### Importar · PCP · Qualidade  
**TOME S/A · Usinagem**

[![APK](https://img.shields.io/badge/Download-Tome__Lider.apk-FF6D00?style=for-the-badge&logo=android&logoColor=white)](./Tome_Lider.apk)
[![Produção](https://img.shields.io/badge/Irmão-APK--PRODUCAO-00C853?style=for-the-badge&logo=github)](https://github.com/ALN2025/APK-PRODUCAO)
[![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)

`com.tome.lider` · **único APK que envia ao PCP**

</div>

---

<br/>

# 🔀 FLUXOGRAMA — SÓ O LÍDER ENVIA AO PCP

> Operadores mandam arquivos → você consolida → **Enviar PCP** / **Enviar Qualidade**

<br/>

```mermaid
%%{init: {
  "theme": "dark",
  "themeVariables": {
    "primaryColor": "#E65100",
    "primaryTextColor": "#fff",
    "primaryBorderColor": "#FFB74D",
    "lineColor": "#90CAF9",
    "secondaryColor": "#1B5E20",
    "tertiaryColor": "#0D47A1",
    "fontSize": "16px"
  }
}}%%
flowchart TB
  subgraph OPS["👷 OPERADORES — APK Produção"]
    O1[Operador A<br/>Diário + R-022]
    O2[Operador B<br/>Diário + R-022]
    O3[Folha OF<br/>quando salvar]
  end

  subgraph LIDER["📱 APK LÍDER — você"]
    IMP[📥 Importar / Receber]
    DADOS[📊 Aba Dados]
    PCP_B[🟢 Enviar PCP]
    QUAL_B[🔵 Enviar Qualidade]
    IMP --> DADOS
    DADOS --> PCP_B
    DADOS --> QUAL_B
  end

  O1 -->|"XLS PDF"| IMP
  O2 -->|"XLS PDF"| IMP
  O3 -.->|"XLS PDF"| IMP

  PCP_B ==> PCP[(🏭 PCP)]
  QUAL_B ==> QUAL[(✅ Qualidade)]
```

<br/>

```mermaid
%%{init: {"theme": "base", "themeVariables": { "fontSize": "16px" }}}%%
flowchart LR
  subgraph in [Entra]
    D[Diários]
    R[R-022]
    F[Folha OF]
  end
  subgraph out [Você envia]
    P[PCP]
    Q[Qualidade]
  end
  D --> P
  R --> Q
  F --> Q
```

<br/>

| Botão no app | Origem | Destino final |
|--------------|--------|---------------|
| **Enviar PCP** | Diários importados | **PCP** |
| **Enviar R-022** | Cotas do dia | **Qualidade** |
| Folha OF | Ordem | **Qualidade** (separado) |

WhatsApp · Telegram · Email

---

## Abas

| Aba | Função |
|-----|--------|
| **Importar** | Bluetooth / receber / arquivo |
| **Dados** | **Enviar PCP** · **Enviar Qualidade** |
| **Códigos** | Só consultar legendas |

---

## Download

### [`Tome_Lider.apk`](./Tome_Lider.apk)

---

## Stack

Flutter · SQLite · excel · pdf · share_plus · flavor `lider`

---

<div align="center">

<img src="aln.png" alt="Dev A.L.N" height="56"/>

### Desenvolvido por **Dev A.L.N**

[github.com/ALN2025](https://github.com/ALN2025) · TOME S/A · 2026

</div>
