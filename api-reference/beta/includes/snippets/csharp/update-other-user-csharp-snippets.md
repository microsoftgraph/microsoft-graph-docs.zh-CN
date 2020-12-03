---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4caf7eccf501a13c9b9d9c18c3136811051b3ad
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556228"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    BusinessPhones = new List<String>()
    {
        "+1 425 555 0109"
    },
    OfficeLocation = "18/2111"
};

await graphClient.Users["{id}"]
    .Request()
    .UpdateAsync(user);

```