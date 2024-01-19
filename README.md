# biome-ignore-unknown-bug

REPRODUCTION:

1. run `npm install`
2. run `npx @biomejs/biome format .` - see that `/src/exclude/.eslintrc` would be formatted, despite not being in the `include` list
3. remove `"ignoreUnknown": true,` from the biome.json
4. run `npx @biomejs/biome format .` again. - see that `/src/exclude/.eslintrc` is now excluded
