---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21cb10b39fc2dc0370b8437bb18b087fb5440f62
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = new AccessReviewScheduleDefinition
{
    DisplayName = "Review employee access to LinkedIn",
    DescriptionForAdmins = "Review employee access to LinkedIn",
    Scope = new PrincipalResourceMembershipsScope
    {
        PrincipalScopes = new List<AccessReviewScope>()
        {
            new AccessReviewQueryScope
            {
                Query = "/users",
                QueryType = "MicrosoftGraph"
            }
        },
        ResourceScopes = new List<AccessReviewScope>()
        {
            new AccessReviewQueryScope
            {
                Query = "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
                QueryType = "MicrosoftGraph"
            }
        }
    },
    Reviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "./manager",
            QueryType = "MicrosoftGraph",
            QueryRoot = "decisions"
        }
    },
    BackupReviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
            QueryType = "MicrosoftGraph"
        }
    },
    FallbackReviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
            QueryType = "MicrosoftGraph"
        }
    },
    Settings = new AccessReviewScheduleSettings
    {
        MailNotificationsEnabled = true,
        ReminderNotificationsEnabled = true,
        JustificationRequiredOnApproval = true,
        DefaultDecisionEnabled = true,
        DefaultDecision = "Recommendation",
        InstanceDurationInDays = 180,
        AutoApplyDecisionsEnabled = true,
        RecommendationsEnabled = true,
        Recurrence = new PatternedRecurrence
        {
            Pattern = new RecurrencePattern
            {
                Type = RecurrencePatternType.AbsoluteMonthly,
                Interval = 6,
                DayOfMonth = 0
            },
            Range = new RecurrenceRange
            {
                Type = RecurrenceRangeType.Numbered,
                StartDate = new Date(2021,5,5),
                EndDate = new Date(2022,5,5)
            }
        }
    }
};

await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .AddAsync(accessReviewScheduleDefinition);

```