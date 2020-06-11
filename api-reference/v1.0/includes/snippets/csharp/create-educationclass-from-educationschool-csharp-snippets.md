---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86e4ab4845250cf87e326e77650f34f2ddae7d86
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684492"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/education/classes/11006"}
    }
};

await graphClient.Education.Schools["{school-id}"].Classes.References
    .Request()
    .AddAsync(educationClass);

```