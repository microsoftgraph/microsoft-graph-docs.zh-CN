---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5fbc5373bf748c9f01733db885e5fd36b60f15
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var regionalAndLanguageSettings = new RegionalAndLanguageSettings
{
    DefaultDisplayLanguage = new LocaleInfo
    {
        Locale = "en-US"
    },
    AuthoringLanguages = new List<LocaleInfo>()
    {
        new LocaleInfo
        {
            Locale = "fr-FR"
        },
        new LocaleInfo
        {
            Locale = "de-DE"
        }
    },
    DefaultTranslationLanguage = new LocaleInfo
    {
        Locale = "en-US"
    },
    DefaultSpeechInputLanguage = new LocaleInfo
    {
        Locale = "en-US"
    },
    DefaultRegionalFormat = new LocaleInfo
    {
        Locale = "en-GB"
    },
    RegionalFormatOverrides = new RegionalFormatOverrides
    {
        Calendar = "Gregorian Calendar",
        FirstDayOfWeek = "Sunday",
        ShortDateFormat = "yyyy-MM-dd",
        LongDateFormat = "dddd, MMMM d, yyyy",
        ShortTimeFormat = "HH:mm",
        LongTimeFormat = "h:mm:ss tt",
        TimeZone = "Pacific Standard Time"
    }
};

await graphClient.Me.Settings.RegionalAndLanguageSettings
    .Request()
    .PutAsync(regionalAndLanguageSettings);

```