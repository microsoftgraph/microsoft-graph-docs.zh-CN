---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d80d7f1ec3bb2f1aafd4a82cd2b913ff810186ff
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/education/users/13015"}
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Members.References
    .Request()
    .AddAsync(educationUser);

```