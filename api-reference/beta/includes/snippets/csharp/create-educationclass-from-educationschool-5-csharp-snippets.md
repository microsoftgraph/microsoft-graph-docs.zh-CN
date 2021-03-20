---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8689ece67ce7fef04bc33634961ab495df8a4c8b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951296"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/education/classes/11006"}
    }
};

await graphClient.Education.Schools["{educationSchool-id}"].Classes.References
    .Request()
    .AddAsync(educationClass);

```