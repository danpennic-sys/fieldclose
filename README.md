# FieldClose

Offline quote-to-invoice closer for trades. Built to sit on the FieldQuote asset pack (Operator Pages).

FieldQuote shipped templates and scripts. FieldClose is the software that fills them, prints the paper, and writes a canonical receipt JSON with a SHA-256 checksum.

It does **not** sign evidence. QuantumGuard remains the only verifier. A FieldClose hash is a checksum you can seal later. It is not an Ed25519 signature and it is not post-quantum.

## Sell

| Tier | Price | What the buyer gets |
|------|------:|---------------------|
| Operator | $349 | This app + FieldQuote Operator templates |
| Command | $1,497 | Operator + branding, scripts, onboarding call |

Open `fieldclose.html` in a browser. No install. No account. Data stays in the browser unless the operator downloads the receipt.

## Honest limits

- Local only. No Stripe, no email send, no accounting sync.
- Checksum, not a signature. Do not market this as QuantumGuard.
- Prices match the FieldQuote pack already in `danpennic-sys/fieldquote`. Do not invent a third price sheet.
