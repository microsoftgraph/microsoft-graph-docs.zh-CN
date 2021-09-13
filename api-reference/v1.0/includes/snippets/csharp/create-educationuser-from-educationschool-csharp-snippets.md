---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 269787e8fe23edcadf399d71b698220558ae52ddeccc79d89471fb368addcf51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277162"
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