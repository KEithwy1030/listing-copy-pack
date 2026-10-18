# Amazon / Shopify / eBay Listing Copy Pack

Apify Actor that turns **product facts** into ready-to-paste **English listing copy**:

- 3 title options (A/B ready)
- Up to 6 benefit bullets
- Short description
- 2 FAQ rows

Deterministic templates — **no LLM, no network, no API key**.

- **Run on Apify Store:** https://apify.com/keiwy/listing-copy-pack
- **Price:** Pay per event — **$0.10** per successful pack (`listing-pack-generated`)
- **Sample input:** [`sample_input.json`](./sample_input.json)
- **Sample output:** [`sample_output.json`](./sample_output.json)
- **Gist:** https://gist.github.com/KEithwy1030/fa6008e8ea2047a5c46b588ccd763539

- **Landing (GitHub Pages):** https://keithwy1030.github.io/listing-copy-pack/
- **Write-up:** https://telegra.ph/Amazon-Shopify-eBay-Listing-Copy-Pack--010-10-18

## Quick try

1. Open the Store link
2. Paste the sample JSON (or your own product facts)
3. Run → read the dataset item (titles / bullets / description / faq)

## Input fields

| Field | Required | Notes |
|-------|----------|-------|
| `product_name` | yes | Primary keyword + product type |
| `audience` | no | Who buys it |
| `category` | no | Amazon/Shopify category hint |
| `primary_benefit` | no | Lead benefit for title A |
| `tone` | no | Voice guidance |
| `facts` | no | `\|`-separated, array, or one fact per line |

## Who this is for

Amazon FBA / Seller Central, Shopify, and eBay sellers who need a first-pass listing pack without hiring a copywriter.
