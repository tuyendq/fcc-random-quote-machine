# freeCodeCamp - Random Quote Machine

## Deploy to surge.sh

- Check available domain
  1quote.surge.sh

```powershell
$REPO_NAME = "fcc-random-quote-machine"
$SURGE_DOMAIN = "1quote.surge.sh"
$SURGE_TOKEN = surge token

# Set domain you want to publish your site on https://your-surge-website-or-custom-domain.surge.sh
gh secret set SURGE_DOMAIN -b"${SURGE_DOMAIN}" --repos="${REPO_NAME}"

# Set secret visible only to certain repositories
gh secret set SURGE_TOKEN --body="${SURGE_TOKEN}" --repos="${REPO_NAME}"
```

- Compose .github/workflows/publish-surge.yaml file
