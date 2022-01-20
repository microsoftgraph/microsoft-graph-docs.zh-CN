---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: faedc0e173d1f17615bf34d684dfc8e83bfa0285
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    CustomSecurityAttributes = new CustomSecurityAttributeValue
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"Engineering", "{\"@odata.type\":\"#Microsoft.DirectoryServices.CustomSecurityAttributeValue\",\"ProjectDate\":\"2022-10-01\"}"}
        }
    }
};

await graphClient.Users["{user-id}"]
    .Request()
    .UpdateAsync(user);

```