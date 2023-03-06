# genshin-db-dist

The plan:

genshin-db sends a private dispatch event whenever a new release is made.

genshin-db-dist will catch the event and trigger the workflow:

- clone genshin-db
- npm run assemble and copy over data.min.json and data.min.json.gzip
- npm run buildAll and copy over the gzips and scripts folder
