---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d41b0b994b90d0a862bcc57dee3482c755f73e45
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = new EducationRubric
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"}
    }
};

await graphClient.Education.Classes["{id}"].Assignments["{id}"].Rubric.Reference
    .Request()
    .PutAsync(educationRubric);

```