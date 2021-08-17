---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54e6de5c687dbc2db572b376c92346dbb9cd9dc3e110fe6de23d7345833a6cc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279426"
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