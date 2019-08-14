---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d54d3d2cef8ab1acb7933f18975d137a14eaf312
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396826"
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

await graphClient.Me
    .Request()
    .UpdateAsync(user);

```