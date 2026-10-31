# CareFlow

Lembretes de medicação para Android. Importa planos de tratamento a partir de PDF, permite vários tratamentos ativos e agenda alarmes nativos que tocam mesmo com a app fechada (com botões **Tomei**, **Adiar 10 min** e **Saltar** na notificação).

## Instalar no telemóvel
1. Abra, no telemóvel, a página **Releases** deste repositório.
2. Descarregue **CareFlow.apk** da versão mais recente.
3. Abra o ficheiro e permita "Instalar apps desconhecidas" quando o Android pedir.
4. Na primeira abertura, autorize as notificações.

## Como é compilada
Cada alteração no ramo `main` é compilada automaticamente pelo GitHub Actions (`.github/workflows/build.yml`) e publicada como nova versão em Releases.

- `www/index.html` — a app (HTML/JS, corre dentro do Capacitor)
- `scripts/patch-android.js` — permissões, ícones, assinatura e versão
- `scripts/parser.js` — leitor offline de planos de posologia
- `res/` — ícones, ecrã inicial e chave de assinatura

> A CareFlow ajuda a lembrar as tomas; não substitui o médico ou o farmacêutico.
