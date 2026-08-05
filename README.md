<div align="center">

<img src="aln.png" alt="Dev A.L.N" height="72"/>

# TOME Líder

### Importar · PCP · Qualidade  
**TOME S/A · Usinagem**

[![APK](https://img.shields.io/badge/Download-Tome__Lider.apk-FF6D00?style=for-the-badge&logo=android&logoColor=white)](./Tome_Lider.apk)
[![Produção](https://img.shields.io/badge/Irmão-APK--PRODUCAO-00C853?style=for-the-badge&logo=github)](https://github.com/ALN2025/APK-PRODUCAO)

`com.tome.lider` · **único APK que envia ao PCP**

</div>

---

<br/>

# 🔀 FLUXO — SÓ O LÍDER ENVIA AO PCP

> Operadores mandam **Diário** e **R-022** para você.  
> **Só você** aperta **Enviar PCP**.

<br/>

```mermaid
%%{init: {
  "theme": "dark",
  "themeVariables": {
    "primaryColor": "#E65100",
    "primaryTextColor": "#fff",
    "primaryBorderColor": "#FFB74D",
    "lineColor": "#90CAF9",
    "fontSize": "16px"
  }
}}%%
flowchart LR
  A[Operador A] -->|Diário + R-022| L[📱 Você — Líder]
  B[Operador B] -->|Diário + R-022| L
  L ==>|"🟢 Enviar PCP<br/>SÓ VOCÊ"| PCP[(🏭 PCP)]
  L -->|"🔵 Qualidade"| Q[(✅ Qualidade)]
  A -.->|"❌ proibido"| PCP
  B -.->|"❌ proibido"| PCP
```

<br/>

```mermaid
%%{init: {
  "theme": "dark",
  "themeVariables": {
    "primaryColor": "#E65100",
    "primaryTextColor": "#fff",
    "primaryBorderColor": "#FFB74D",
    "lineColor": "#90CAF9",
    "fontSize": "15px"
  }
}}%%
flowchart TB
  subgraph OPS["👷 OPERADORES"]
    O1[Diário + R-022 → Líder]
  end
  subgraph LIDER["📱 APK LÍDER"]
    IMP[📥 Importar]
    PCP_B[🟢 Enviar PCP — SÓ VOCÊ]
    QUAL_B[🔵 Enviar Qualidade]
    IMP --> PCP_B
    IMP --> QUAL_B
  end
  O1 --> IMP
  PCP_B ==> PCP[(🏭 PCP)]
  QUAL_B ==> QUAL[(✅ Qualidade)]
```

<br/>

| Botão | O que junta | Destino |
|-------|-------------|---------|
| **Enviar PCP** | Diários | **PCP** — só o líder |
| **Enviar R-022** | Cotas | **Qualidade** |
| Folha OF | Ordem | **Qualidade** (separado) |

---

### [`Tome_Lider.apk`](./Tome_Lider.apk)

<div align="center">
<img src="aln.png" alt="Dev A.L.N" height="56"/>
### Desenvolvido por **Dev A.L.N** · TOME S/A · 2026
</div>
