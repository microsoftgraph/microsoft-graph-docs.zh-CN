---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68c925a8b2302859cb597af1f62ed5fc36b92853
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"ext55gb1l09_msLearnCourses", "{\"courseType\":\"Admin\"}"}
    }
};

await graphClient.Users["{user-id}"]
    .Request()
    .UpdateAsync(user);

```