---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d37e1fa03b1dfbad6b391cc31b466bcead67bf6c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887664"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/education/classes/11006"}
    }
};

await graphClient.Education.Schools["{school-id}"].Classes.References
    .Request()
    .AddAsync(educationClass);

```