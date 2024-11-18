Adapted from: https://github.com/gorhom/react-native-bottom-sheet/pull/1142

In this directory:
```bash
yarn bootstrap
yarn typescript
rm -rf lib && yarn build
```

```bash
yarn patch @gorhom/bottom-sheet
cd /private/path/referenced/by/yarn/patch
cp -a /path/to/react-native-bottom-sheet/src -a /path/to/react-native-bottom-sheet/lib .
# change back to nodejs project we want to apply a yarn patch to
yarn patch-commit -s /private/path/referenced/by/yarn/patch
```