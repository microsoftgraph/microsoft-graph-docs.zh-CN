---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0039d2549a4f362c5d89e12cd36ad86ab13fc74
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const regionalAndLanguageSettings = {
    defaultDisplayLanguage: {
        locale: "en-US"
    },
    authoringLanguages: [
        {
            locale: "fr-FR"
        },
        {
            locale: "de-DE"
        }
    ],
    defaultTranslationLanguage: {
        locale: "en-US"
    },
    defaultSpeechInputLanguage: {
        locale: "en-US"
    },
    defaultRegionalFormat: {
        locale: "en-GB"
    },
    regionalFormatOverrides: {
        calendar: "Gregorian Calendar",
        firstDayOfWeek: "Sunday",
        shortDateFormat: "yyyy-MM-dd",
        longDateFormat: "dddd, MMMM d, yyyy",
        shortTimeFormat: "HH:mm",
        longTimeFormat: "h:mm:ss tt",
        timeZone: "Pacific Standard Time"
    }
};

let res = await client.api('/me/settings/regionalandlanguagesettings')
    .version('beta')
    .put(regionalAndLanguageSettings);

```