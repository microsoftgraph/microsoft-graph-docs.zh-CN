---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b657931f9f13570d4f9ce3c50e7ed1c8e016e0e64b7a849e3f5240f4c027e04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219098"
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