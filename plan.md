this is a revisit of an old project.

I would like to remake it with a new approach:

bootstrap inherent jquery => using percel, webpack etc.

some refreshing mechanism into SPA later on.

check it out.

heder:
navigation and search bar.



bootstrap installation:
https://getbootstrap.com/docs/5.0/getting-started/download/#npm

npm install bootstrap@next
yarn add parcel-bundler --dev
scripts:
    "dev": "parcel ./src/index.html",
    "prebuild": "npx rimraf build",
    "build": "parcel build --public-url ./ ./src/index.html --experimental-scope-hoisting --out-dir ./ ",
    "git": "git add . && git commit -m",
    "postgit": "git push --all"

home page:

hero

retrieved coins

6k coins, minimal data:
https://api.coingecko.com/api/v3/coins/list

full coin details:
https://api.coingecko.com/api/v3/coins/bitcoin


pipe - real coinage such as $
price_current.market_data.usd

0. under the table - make the call for the extended 6K coins.
1 fetch all coins into an array.
2 display coin data : title, image, and the collapser for more info
3 match the selected coin with the full data.

update coin data on intervals.

remade the BS instalation from the orig:
https://github.com/twbs/bootstrap-npm-starter.git
