---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3d8d43aec1603ef0bf24b70b7c22d14bdc921fb
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820284"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPatent = new ItemPatent
{
    Description = "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
    DisplayName = "Inferring User Intent through browsing behaviors",
    IsPending = true,
    Number = "USPTO-3954432633",
    WebUrl = "https://patents.gov/3954432633"
};

await graphClient.Me.Profile.Patents
    .Request()
    .AddAsync(itemPatent);

```