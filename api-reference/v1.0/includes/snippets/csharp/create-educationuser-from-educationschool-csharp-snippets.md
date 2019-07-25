---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dfe27d552f7db17e6b9cf9a11124429f87f44e57
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887636"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/education/users/14008"}
    }
};

await graphClient.Education.Schools["{id}"].Users.References
    .Request()
    .AddAsync(educationUser);

```