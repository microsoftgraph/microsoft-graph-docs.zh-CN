---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c7be88677068fe77536f1a36bcf61db3cde9e08
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683787"
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

await graphClient.Education.Schools["10002"].Classes.References
    .Request()
    .AddAsync(educationClass);

```