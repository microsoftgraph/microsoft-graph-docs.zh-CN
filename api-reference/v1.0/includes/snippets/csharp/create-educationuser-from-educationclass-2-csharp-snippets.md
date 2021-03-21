---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5d5442bccced4460a7ed3a9ba1ceed7c7162536
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963728"
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

await graphClient.Education.Classes["{educationClass-id}"].Teachers.References
    .Request()
    .AddAsync(educationUser);

```