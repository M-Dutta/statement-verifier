# Statement Lookup

This is a plugin that provides more context on statements you read online.
It interacts with Gemini to gather informantion about a selected text.

### Example Images:

|                            Text Selection                            |                             Answer                              |
|:--------------------------------------------------------------------:|:---------------------------------------------------------------:|
| <img src="readme_assets/example-dropdown-option.png" width="100%" /> | <img src="readme_assets/example-screenshot.png" width="100%" /> |

## Compatibility

Chromium

- **manifest** v3

## Development

To start developing, install yarn packages

```bash
yarn install
```

Then run in `dev`

```bash
yarn dev
```

## Making production build

Run the following:

```bash
yarn build
```

should create a build in [build/chrome-mv3-prod](build/chrome-mv3-prod)

### Packaging the build

```bash
yarn package
```

should create a zip in [build/chrome-mv3-prod.zip](build/chrome-mv3-prod.zip)

This is a production bundle the extension, ready to be zipped and published to the stores.

## Loading the extension

1. Download the `statement-lookup-chrome-mv3-<version>.zip` file.
2. Unpack the `.zip` file.
3. Open `Chrome` and navigate to `chrome://extensions/`
4. Click `Load unpacked` button.
5. Navigate to and select the unpacked folder.
   <img src="readme_assets/chrome-extension-loading.png" width="60%"/>
6. Open the plugin options
7. Head over to Google's [AI studio](https://aistudio.google.com/app/apikey) and generate an API key. Copy the key and paste it into the "Gemini Key" block.
   <img src="readme_assets/options-page.png" width="60%"/>

## Credits

> Project is bootstrapped using [Plasmo extension](https://docs.plasmo.com/)