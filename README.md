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

> Operador **pode** mandar Diário e **R-022** a qualquer hora.  
> Você consolida → **Enviar PCP** (só você) / **Enviar Qualidade**.

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
    O1[Operador A<br/>Diário + R-022 ok]
    O2[Operador B<br/>Diário + R-022 ok]
    O3[Folha OF]
  end

  subgraph LIDER["📱 APK LÍDER — você"]
    IMP[📥 Importar / Receber]
    DADOS[📊 Aba Dados]
    PCP_B[🟢 Enviar PCP — SÓ VOCÊ]
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

| Botão no app | Origem | Destino final |
|--------------|--------|---------------|
| **Enviar PCP** | Diários dos operadores | **PCP** (só o líder) |
| **Enviar R-022** | Cotas recebidas | **Qualidade** |
| Folha OF | Ordem | **Qualidade** (separado) |

---

## Abas

| Aba | Função |
|-----|--------|
| **Importar** | Recebe Diário e R-022 dos operadores |
| **Dados** | **Enviar PCP** · **Enviar Qualidade** |
| **Códigos** | Consultar legendas |

---

## Download

### [`Tome_Lider.apk`](./Tome_Lider.apk)

---

<div align="center">

<img src="aln.png" alt="Dev A.L.N" height="56"/>

### Desenvolvido por **Dev A.L.N**

[github.com/ALN2025](https://github.com/ALN2025) · TOME S/A · 2026

</div>
