---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5a4e44b1a8c3f3288cf06936462a4c83be4a850
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/education/users/14008"}
    }
};

await graphClient.Education.Schools["{educationSchool-id}"].Users.References
    .Request()
    .AddAsync(educationUser);

```