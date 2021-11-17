---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 947e69e8718efd4b61af8a526cb4950eb4fedc29e5f5002ea4d44ce16536d0b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const regionalAndLanguageSettings = {
    defaultDisplayLanguage: {
        locale: 'en-US'
    },
    authoringLanguages: [
        {
            locale: 'fr-FR'
        },
        {
            locale: 'de-DE'
        }
    ],
    defaultTranslationLanguage: {
        locale: 'en-US'
    },
    defaultSpeechInputLanguage: {
        locale: 'en-US'
    },
    defaultRegionalFormat: {
        locale: 'en-GB'
    },
    regionalFormatOverrides: {
        calendar: 'Gregorian Calendar',
        firstDayOfWeek: 'Sunday',
        shortDateFormat: 'yyyy-MM-dd',
        longDateFormat: 'dddd, MMMM d, yyyy',
        shortTimeFormat: 'HH:mm',
        longTimeFormat: 'h:mm:ss tt',
        timeZone: 'Pacific Standard Time'
    },
    translationPreferences: {
        translationBehavior: 'Yes',
        languageOverrides: [
            {
                languageTag: 'fr',
                translationBehavior: 'Yes' 
            }
        ]
     }
};

await client.api('/me/settings/regionalandlanguagesettings')
    .version('beta')
    .put(regionalAndLanguageSettings);

```