---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81db0bb29fe3ac268302e8102087aea9e2f1a6ab
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201456"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var adminConsentRequestPolicy = new AdminConsentRequestPolicy
{
    IsEnabled = true,
    NotifyReviewers = true,
    RemindersEnabled = true,
    RequestDurationInDays = 5,
    Reviewers = new List<AccessReviewScope>()
    {
        new AccessReviewScope
        {
            Query = "/users/b6879be8-fb87-4482-a72e-18445d2b5c54",
            QueryType = "MicrosoftGraph"
        },
        new AccessReviewScope
        {
            Query = "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9",
            QueryType = "MicrosoftGraph"
        }
    }
};

await graphClient.Policies.AdminConsentRequestPolicy
    .Request()
    .PutAsync(adminConsentRequestPolicy);

```