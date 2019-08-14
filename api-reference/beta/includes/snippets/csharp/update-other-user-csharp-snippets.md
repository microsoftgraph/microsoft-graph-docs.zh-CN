---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a77b2874d4e70f79d99c00d0a9895bee1bcb4f80
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    BusinessPhones = new List<String>()
    {
        "businessPhones-value"
    },
    OfficeLocation = "city-value"
};

await graphClient.Users["{id}"]
    .Request()
    .UpdateAsync(user);

```