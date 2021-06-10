---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f14e3306c04c3c78960c229a1335728c403b67ea
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871377"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = new AccessReviewScheduleDefinition
{
    DisplayName = "Review inactive guests on teams",
    DescriptionForAdmins = "Control guest user access to our teams.",
    DescriptionForReviewers = "Information security is everyone's responsibility. Review our access policy for more.",
    InstanceEnumerationScope = new AccessReviewQueryScope
    {
        Query = "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
        QueryType = "MicrosoftGraph"
    },
    Scope = new AccessReviewInactiveUsersQueryScope
    {
        Query = "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
        QueryType = "MicrosoftGraph",
        InactiveDuration = new Duration("P30D")
    },
    Reviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "./owners",
            QueryType = "MicrosoftGraph"
        }
    },
    FallbackReviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
            QueryType = "MicrosoftGraph"
        }
    },
    Settings = new AccessReviewScheduleSettings
    {
        MailNotificationsEnabled = true,
        ReminderNotificationsEnabled = true,
        JustificationRequiredOnApproval = true,
        RecommendationsEnabled = true,
        InstanceDurationInDays = 3,
        Recurrence = new PatternedRecurrence
        {
            Pattern = new RecurrencePattern
            {
                Type = RecurrencePatternType.AbsoluteMonthly,
                DayOfMonth = 5,
                Interval = 3
            },
            Range = new RecurrenceRange
            {
                Type = RecurrenceRangeType.NoEnd,
                StartDate = new Date(2020,5,4)
            }
        },
        DefaultDecisionEnabled = true,
        DefaultDecision = "Deny",
        AutoApplyDecisionsEnabled = true
    }
};

await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .AddAsync(accessReviewScheduleDefinition);

```