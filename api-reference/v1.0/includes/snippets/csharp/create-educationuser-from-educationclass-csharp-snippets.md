---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c05d585380c101458fb909b6e2edbb3e8f552b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/education/users/13015"}
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Members.References
    .Request()
    .AddAsync(educationUser);

```