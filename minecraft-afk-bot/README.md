# Minecraft AFK Bot

بوت محلي يحافظ على اتصال حساب Minecraft بسيرفر مصرح به، مع دعم منفصل لـ **Java Edition** و**Bedrock Edition**.

> استعمله فقط في سيرفر تملكه أو يسمح صراحةً بالـAFK bots. لا يهدف لتجاوز تسجيل الدخول أو قوانين السيرفرات.

## Server configuration

```text
Host: ARBICSMP.aternos.me
Port: 16503
Platform: PaperMC / Java or a Bedrock bridge
```

## Install

يحتاج المشروع إلى Node.js 18 أو أحدث. لا تضع كلمات السر أو رموز الدخول داخل GitHub.

```bash
npm install
cp .env.example .env
```

## Java Edition

```bash
npm run java
```

يعيد البوت الاتصال بعد الانقطاع ويقوم بحركة AFK خفيفة. الإعداد `MC_AUTH=offline` مناسب فقط للسيرفرات التي تسمح بالدخول offline-mode.

## Bedrock Edition

```bash
npm run bedrock
```

يحتاج Bedrock إلى منفذ Bedrock فعلي أو Bridge مثل Geyser؛ منفذ Java وحده لا يكفي عادةً. استعمل منفذ Bedrock الذي يعرضه صاحب السيرفر.

## Environment variables

| Variable | Example | Description |
|---|---|---|
| `MC_HOST` | `ARBICSMP.aternos.me` | Server hostname |
| `MC_PORT` | `16503` | Java or Bedrock port |
| `MC_USERNAME` | `KAMAL_AFK_BOT` | Bot username |
| `MC_AUTH` | `offline` | Authentication mode allowed by the server |
| `MC_VERSION` | `1.21.1` | Java version |
| `MC_BEDROCK_VERSION` | `1.21.0` | Bedrock protocol version |
| `AFK_INTERVAL_MS` | `45000` | Movement interval in milliseconds |

## Safety

شغّل البوت فقط في سيرفر تملكه أو لديك إذن واضح باستعماله. لا تستعمله للغش أو لتجاوز الحظر أو المصادقة، وراجع قوانين Aternos وPaperMC قبل التشغيل.
