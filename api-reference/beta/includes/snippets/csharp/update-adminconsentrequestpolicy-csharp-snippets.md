---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06f4f140ab2adb639554cfdbfd1c9e4de38a256fc6c0040f5a7f9ad78bf2dcb5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104091"
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