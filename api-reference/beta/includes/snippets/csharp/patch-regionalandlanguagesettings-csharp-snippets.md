---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87b8b0acdfc44b55935029f569af50b70d87e0cf
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var regionalAndLanguageSettings = new RegionalAndLanguageSettings
{
    AuthoringLanguages = new List<LocaleInfo>()
    {
        new LocaleInfo
        {
            Locale = "en-US"
        },
        new LocaleInfo
        {
            Locale = "es-MX"
        }
    },
    DefaultRegionalFormat = new LocaleInfo
    {
        Locale = "en-US"
    }
};

await graphClient.Me.Settings.RegionalAndLanguageSettings
    .Request()
    .UpdateAsync(regionalAndLanguageSettings);

```