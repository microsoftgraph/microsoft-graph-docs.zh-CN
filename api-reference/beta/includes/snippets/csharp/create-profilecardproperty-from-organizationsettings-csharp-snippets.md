---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a0380cad867628b8e287766045891f473f17596
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566645"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperty = new ProfileCardProperty
{
    DirectoryPropertyName = "CustomAttribute1",
    Annotations = new List<ProfileCardAnnotation>()
    {
        new ProfileCardAnnotation
        {
            DisplayName = "Cost Center",
            Localizations = new List<DisplayNameLocalization>()
            {
                new DisplayNameLocalization
                {
                    LanguageTag = "ru-RU",
                    DisplayName = "центр затрат"
                }
            }
        }
    }
};

await graphClient.Organization["{organizationId}"].Settings.ProfileCardProperties
    .Request()
    .AddAsync(profileCardProperty);

```