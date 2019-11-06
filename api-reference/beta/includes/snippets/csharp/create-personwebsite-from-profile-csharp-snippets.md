---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba739f2e4aca36fb4c1769d0310b8056ad6d9e6e
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personWebsite = new PersonWebsite
{
    Categories = new List<String>()
    {
        "categories-value"
    },
    Description = "description-value",
    DisplayName = "displayName-value",
    WebUrl = "webUrl-value"
};

await graphClient.Me.Profile.Websites
    .Request()
    .AddAsync(personWebsite);

```