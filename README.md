# Installation / Configuration

## Using JQ

```
pkg=$(jq '.prettier="@bitboxx/prettier-config" | .devDependencies["eslint-config-bitboxx"]="github:bitboxx/eslint-config-bitboxx"' package.json) && \
  echo -E "$pkg" > package.json

yarn
```

## Manual Installation

```
yarn add --dev @bitboxx/prettier-config@github:bitboxx/prettier-config.git
```

```
// package.json

{
  // ...
  "prettier": "@bitboxx/prettier-config"
}
```
