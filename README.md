# HTTPS Everywhere Builder

Builds HTTPS Everywhere ruleset files for Veera.

## Configuring

If there are rulesets that are broken and need to be disabled, add them to the `exclusions` list.

## Building locally

    npm install
    npm run build

## Testing locally

1. Copy `out/httpse.leveldb.zip` into `~/.config/BraveSoftware/Brave-Browser-Beta/imifmkfbgdbjflacljaiepbebjdpllai/*/*/` overwriting the existing file.
2. Delete the `httpse.leveldb` directory.
3. Unzip `httpse.leveldb.zip`.
4. Start the browser and ensure that <http://https-everywhere.badssl.com/> works.
5. Find a site that was added in the last release and check that it gets upgraded. Check it first with `curl --head` to make sure it doesn't redirect to HTTPS server-side.

## Releasing a new version

1.Contact Veera Team
