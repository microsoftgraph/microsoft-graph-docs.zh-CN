---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48e4531e0b2826e89b4e4098c1d5e6be94e1c697
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997814"
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

await graphClient.Me.Profile.Interests
    .Request()
    .AddAsync(personInterest);

```