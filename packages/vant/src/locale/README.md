# Internationalization

### Intro

Vant uses Chinese as the default language. If you want to use other languages, please follow the instructions below.

## Usage

### Switch languages

Vant supports multiple languages with the Locale component, and the `Locale.use` method allows you to switch to different languages.

```js
import { Locale } from 'vant';
import enUS from 'vant/es/locale/lang/en-US';

Locale.use('en-US', enUS);
```

### Override default configs

Use `Locale.add` method to modify the default configs.

```js
import { Locale } from 'vant';

const messages = {
  'en-US': {
    vanPicker: {
      confirm: 'Close',
    },
  },
};

Locale.add(messages);
```

### Config files

Current supported languages:

| Language                 | Filename     |
| ------------------------ | ------------ |
| German                   | de-DE        |
| German (formal)          | de-DE-formal |
| English                  | en-US        |
| Spanish (Spain)          | es-ES        |
| French                   | fr-FR        |
| Hindi                    | hi-IN        |
| Japanese                 | ja-JP        |
| Korean                   | ko-KR        |
| Norwegian                | nb-NO        |
| Portuguese (Brazil)      | pt-BR        |
| Romanian                 | ro-RO        |
| Russian                  | ru-RU        |
| Turkish                  | tr-TR        |
| Thai                     | th-TH        |
| Chinese                  | zh-CN        |
| Traditional Chinese (HK) | zh-HK        |
| Traditional Chinese (TW) | zh-TW        |

> View all language configs [Here](https://github.com/youzan/vant/tree/dev/packages/vant/src/locale/lang).

### Add new language

If you can’t find the language you need, please send us a Pull Request to add the new language pack, you can refer to [Add German language pack](https://github.com/youzan/vant/pull/7245) PR.
