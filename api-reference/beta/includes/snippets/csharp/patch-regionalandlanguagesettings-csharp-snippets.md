---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15071991c2d3e848c8b1c52c4ff3c0e76ec31bd49f64e493fb04eee8a7c1b968
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219100"
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