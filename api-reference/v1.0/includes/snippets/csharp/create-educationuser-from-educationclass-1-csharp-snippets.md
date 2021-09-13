---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3ee79f7f56311a451f8852b7ab2362d532640daf5781d574143084ac2c2a174
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/education/users/13015"}
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Members.References
    .Request()
    .AddAsync(educationUser);

```