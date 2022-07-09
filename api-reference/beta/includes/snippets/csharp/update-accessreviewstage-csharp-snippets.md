---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e5379c9938ea00b0f1f4c0b27ac168fd692bd9c
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewStage = new AccessReviewStage
{
    Reviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
            QueryType = "MicrosoftGraph"
        }
    },
    FallbackReviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
            QueryType = "MicrosoftGraph"
        },
        new AccessReviewReviewerScope
        {
            Query = "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
            QueryType = "MicrosoftGraph"
        }
    }
};

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Stages["{accessReviewStage-id}"]
    .Request()
    .UpdateAsync(accessReviewStage);

```