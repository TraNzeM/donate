# Donate — страница поддержки

[![Donate](https://img.shields.io/badge/Donate-Support%20me-ff69b4?style=for-the-badge)](https://tranzem.github.io/donate/)

Страница сбора донатов на GitHub Pages: криптовалюта (USDT TRC20, BTC, ETH, TON) + ЮMoney.

URL: **https://tranzem.github.io/donate/**

## Как поменять адреса

Открой `index.html`, в самом начале `<script>` блок `CONFIG`:

```js
const CONFIG = {
  yoomoney: "",      // https://yoomoney.ru/to/4100XXXXXXXXXX
  usdtTrc20: "",     // адрес USDT (TRC20)
  btc: "",           // адрес BTC
  eth: "",           // адрес ETH
  ton: ""            // адрес TON
};
```

Пустое поле = карточка автоматически скрывается. После правки — commit + push, страница обновится сама (GitHub Pages).

## Как подключить к своим репозиториям

**1. Кнопка Sponsor в шапке репо** — скопируй `.github/FUNDING.yml` в свой репозиторий:

```yaml
custom: ["https://tranzem.github.io/donate/"]
```

**2. Бейдж в README:**

```markdown
[![Donate](https://img.shields.io/badge/Donate-Support%20me-ff69b4?style=for-the-badge)](https://tranzem.github.io/donate/)
```

## Технически

- Чистый HTML+CSS+JS, без сборки и зависимостей (QR — через api.qrserver.com).
- Тёмная тема, адаптив, кнопки «Скопировать» (clipboard + fallback) и QR-модалка (Esc/клик мимо — закрыть).
- Токены/ключи не нужны.
