---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5fdbf4d2bddbf23e62dd99eae8954f6cb972dcb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789133"
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
    },
    TranslationPreferences = new TranslationPreferences
    {
        TranslationBehavior = TranslationBehavior.Yes,
        LanguageOverrides = new List<TranslationLanguageOverride>()
        {
            new TranslationLanguageOverride
            {
                LanguageTag = "fr",
                TranslationBehavior = TranslationBehavior.Yes
            }
        }
    }
};

await graphClient.Me.Settings.RegionalAndLanguageSettings
    .Request()
    .PutAsync(regionalAndLanguageSettings);

```