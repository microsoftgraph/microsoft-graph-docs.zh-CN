---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63cac942f1ba82b851de364e8a85b014fb2b8f11
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperty = new ProfileCardProperty
{
    Annotations = new List<ProfileCardAnnotation>()
    {
        new ProfileCardAnnotation
        {
            Localizations = new List<DisplayNameLocalization>()
            {
                new DisplayNameLocalization
                {
                    LanguageTag = "no-NB",
                    DisplayName = "Kostnads Senter"
                }
            }
        }
    }
};

await graphClient.Organization["{organizationId}"].Settings.ProfileCardProperties["CustomAttribute1"]
    .Request()
    .UpdateAsync(profileCardProperty);

```