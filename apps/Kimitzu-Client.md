---
layout: app

permalink: /Kimitzu-Client/
description: Kimitzu Client

icons:
  - Kimitzu-Client/icons/128x128/kimitzu-client.png

screenshots:
  - Kimitzu-Client/screenshot.png

authors:
  - name: kimitzu
    url: https://github.com/kimitzu

links:
  - type: GitHub
    url: kimitzu/kimitzu-client
  - type: Download
    url: https://github.com/kimitzu/kimitzu-client/releases

desktop:
  Desktop Entry:
    Name: Kimitzu Client
    Exec: AppRun
    Terminal: false
    Type: Application
    Icon: kimitzu-client
    StartupWMClass: Kimitzu Client
    X-AppImage-Version: 0.4.0-beta
    Comment: Kimitzu Client
    Categories: Development
  AppImageHub:
    X-AppImage-Signature: no valid OpenPGP data found. the signature could not be verified.
      Please remember that the signature file (.sig or .asc) should be the first file
      given on the command line.
    X-AppImage-Type: 2
    X-AppImage-Architecture: x86_64

electron:
  author:
    email: dev@kimitzu.ch
    name: Kimitzu Foundation
    url: https://github.com/kimitzu
  repository:
    type: git
    url: https://github.com/kimitzu/kimitzu-client.git
  dependencies:
    "@celebryts/react-autocomplete-tags": "^1.0.0"
    "@types/faker": "^4.1.5"
    "@types/jest": "^24.0.12"
    "@types/node": "^12.0.0"
    "@types/qrcode.react": "^0.8.2"
    "@types/react": "^16.8.17"
    "@types/react-dom": "^16.8.4"
    "@types/react-router-dom": "^4.3.3"
    "@types/react-star-rating-component": "^1.4.0"
    "@types/react-tagsinput": "^3.19.3"
    axios: "^0.18.0"
    babel-jest: 24.7.1
    classnames: "^2.2.6"
    create-react-class: "^15.6.3"
    cross-env: "^5.2.0"
    currency-symbol-map: "^4.0.4"
    cypress-file-upload: "^3.3.4"
    electron-is-dev: "^1.1.0"
    electron-log: "^3.0.8"
    electron-serve: "^0.3.0"
    electron-updater: "^4.1.2"
    faker: "^4.1.0"
    is-electron: "^2.2.0"
    iso-639-1: "^2.0.5"
    moment: "^2.24.0"
    multiselect-react-dropdown: "^1.2.8"
    qrcode.react: "^0.9.3"
    react: "^16.8.6"
    react-country-flag: "^1.0.2"
    react-dnd: 5.0.0
    react-dnd-html5-backend: 3.0.2
    react-dom: "^16.3.1"
    react-flip-move: "^3.0.3"
    react-markdown: "^4.2.2"
    react-mde: "^7.6.2"
    react-router-dom: "^5.0.0"
    react-scripts: 3.0.0
    react-select: "^3.0.5"
    react-select-search: "^0.9.6"
    react-slider: "^0.11.2"
    react-star-rating-component: "^1.4.1"
    react-tag-autocomplete: "^5.11.1"
    react-tag-input: "^6.4.0"
    react-tagsinput: "^3.19.0"
    react-textarea-autosize: "^7.1.0"
    react-token-autocomplete: "^0.5.3"
    search-index: "^1.0.6"
    serve: "^11.2.0"
    slugify: "^1.3.4"
    spinkit: "^1.2.5"
    throttle: "^1.0.3"
    typescript: "^3.4.5"
    uikit: "^3.2.3"
    use-force-update: "^1.0.6"
    wait-on: "^3.3.0"
  browserslist:
    production:
    - ">0.2%"
    - not dead
    - not op_mini all
    development:
    - last 1 chrome version
    - last 1 firefox version
    - last 1 safari version
  description: Kimitzu Client
  main: public/electron.js
  homepage: "./"
  husky:
    hooks:
      pre-commit: lint-staged
      pre-push: lint-staged
  lint-staged:
    "*.{ts,tsx}":
    - tslint -c tslint.json
  config:
    commitizen:
      path: "./node_modules/cz-conventional-changelog"
---
