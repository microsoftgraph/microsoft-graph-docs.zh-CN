---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29357a14efe49bc5e3512a278fbe20c5f51166b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785685"
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

await graphClient.Organization["{organization-id}"].Settings.ProfileCardProperties
    .Request()
    .AddAsync(profileCardProperty);

```