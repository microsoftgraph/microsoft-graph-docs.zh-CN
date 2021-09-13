---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ea6b944dec9fe4b8ea271adde13463eaa593d06dbb5c32aa4ef1dfbe6efd283
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106289"
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