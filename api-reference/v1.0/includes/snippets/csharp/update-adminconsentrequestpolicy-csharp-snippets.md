---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdc1768c6d34ba8a05c8185672b0f173aad41d3c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var adminConsentRequestPolicy = new AdminConsentRequestPolicy
{
    IsEnabled = true,
    NotifyReviewers = true,
    RemindersEnabled = true,
    RequestDurationInDays = 5,
    Reviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/users/b6879be8-fb87-4482-a72e-18445d2b5c54",
            QueryType = "MicrosoftGraph"
        },
        new AccessReviewReviewerScope
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