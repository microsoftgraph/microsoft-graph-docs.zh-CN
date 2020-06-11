---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 787a2ac53fbae987540252b9d160054460f23551
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684140"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/education/users/14011"}
    }
};

await graphClient.Education.Classes["{class-id}"].Teachers.References
    .Request()
    .AddAsync(educationUser);

```