---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c04c26adda76f76f4e2748443833f6048e696300
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personInterest = new PersonInterest
{
    Categories = new List<String>()
    {
        "categories-value"
    },
    Description = "description-value",
    DisplayName = "displayName-value",
    WebUrl = "webUrl-value"
};

await graphClient.Me.Profile.Interests["{id}"]
    .Request()
    .UpdateAsync(personInterest);

```