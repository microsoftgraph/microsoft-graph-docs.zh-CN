---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bf231d1cb03f9dbb1f769ef344085d45d1d002c699aa7c5bd1a72f38b7cddf8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewHistoryDefinition = new AccessReviewHistoryDefinition
{
    DisplayName = "Last quarter's group reviews April 2021",
    Decisions = new List<AccessReviewHistoryDecisionFilter>()
    {
        AccessReviewHistoryDecisionFilter.Approve,
        AccessReviewHistoryDecisionFilter.Deny,
        AccessReviewHistoryDecisionFilter.DontKnow,
        AccessReviewHistoryDecisionFilter.NotReviewed,
        AccessReviewHistoryDecisionFilter.NotNotified
    },
    ReviewHistoryPeriodStartDateTime = DateTimeOffset.Parse("2021-01-01T00:00:00Z"),
    ReviewHistoryPeriodEndDateTime = DateTimeOffset.Parse("2021-04-05T00:00:00Z"),
    Scopes = new List<AccessReviewScope>()
    {
        new AccessReviewQueryScope
        {
            QueryType = "MicrosoftGraph",
            Query = "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
            QueryRoot = null
        },
        new AccessReviewQueryScope
        {
            QueryType = "MicrosoftGraph",
            Query = "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
            QueryRoot = null
        }
    }
};

await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions
    .Request()
    .AddAsync(accessReviewHistoryDefinition);

```