# CloudFlare like DynDNS

The main idea of this project is to update DNS registry when my public IP is changed. So you can set this process to run every time you like in order to keep DNS updated.

## Export variables

Create a env.sh file to export the variables:

```bash
export CF_API_KEY="YOUR_API_KEY_TOKEN"
export CF_ZONE_ID="YOUR_ZONE_ID"
export CF_RECORD_ID="YOUR_RECORD_ID"
export CF_RECORD_NAME="YOUR_SUBDOMAIN"
```

And export all variables, like:

```bash
source env.sh
```

## Set priviledges

```bash
chmod +x cf_updateDNS
```

## Run it

```bash
./cf_updateDNS
```
