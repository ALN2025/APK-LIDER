# TOME Líder

APK do **líder** (celular particular) — recebe produção, gera relatórios PCP e Qualidade — TOME S/A.

Repositório: [ALN2025/APK-LIDER](https://github.com/ALN2025/APK-LIDER)

APK irmão (produção): [ALN2025/APK-PRODUCAO](https://github.com/ALN2025/APK-PRODUCAO)

---

## Download

Arquivo de instalação:

**[Tome_Lider.apk](./Tome_Lider.apk)**

Pacote: `com.tome.lider`

---

## Para que serve

| Aba | Função |
|-----|--------|
| **Importar** | Receber arquivos dos operadores (Bluetooth / direto / XLS / PDF) |
| **Dados** | Ver produção importada e gerar **PDF/XLS** |
| **Códigos** | Só para **consultar** o significado das legendas (parada, sucata, operações, roteiro OF). **Não** é relatório nem horas negativas |

### Relatórios (aba Dados)

| Botão / arquivo | Destino |
|-----------------|---------|
| **PCP** (Diário) | Planejamento / produção do dia |
| **R-022** | Qualidade — planilha **do dia** |
| **Folha OF** | Qualidade — fim da OF (**não junta** com o R-022) |

Envio ao time: WhatsApp / Telegram / Email (a partir do celular do líder).

---

## Instalação (Android)

1. Desinstale a versão antiga (se houver).
2. Ative instalar apps desconhecidos.
3. Abra o `Tome_Lider.apk` e instale.
4. Entre com **Nome + Setor**.

Arquivos gerados em geral em `Download/Tome`.

---

## Fluxo prático

1. Operador envia Diário / R-022 / Folha OF (arquivos **separados**).
2. Líder: **Importar** ou **Receber direto**.
3. Aba **Dados** → gerar PDF/XLS PCP ou Qualidade.
4. Aba **Códigos** → só consulta de legendas.

---

## Compilar (desenvolvimento)

```bash
cd tome_producao
flutter pub get
flutter build apk --release --flavor lider --dart-define=FLAVOR=lider
```

Saída: `build/app/outputs/flutter-apk/app-lider-release.apk`

---

## Créditos

TOME S/A · 2026
