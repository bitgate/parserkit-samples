# parserkit samples

Fictional documents for trying the [parserkit](https://parserkit.com) document parsing API. Every company, person and number in them is made up.

| File | What it is |
|---|---|
| [`invoice-fernhill-1004.pdf`](invoice-fernhill-1004.pdf) | US invoice, 4 lines, 10.35% sales tax, $1,743.53 due |
| [`invoice-fernhill-1007.pdf`](invoice-fernhill-1007.pdf) | US invoice, 2 lines, 10.35% sales tax, $780.17 due |
| [`invoice-fernhill-1008.pdf`](invoice-fernhill-1008.pdf) | US invoice, 3 lines, 10.35% sales tax, $1,473.17 due |
| [`invoice-fernhill-1011.pdf`](invoice-fernhill-1011.pdf) | US invoice, 3 lines, 10.35% sales tax, $833.14 due |

## Parse one

```bash
curl https://api.parserkit.com/v1/parse \
  -H "Authorization: Bearer $PARSERKIT_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{"file_url": "https://raw.githubusercontent.com/bitgate/parserkit-samples/master/invoice-fernhill-1004.pdf", "preset": "invoice"}'
```

Docs: https://parserkit.com/docs
