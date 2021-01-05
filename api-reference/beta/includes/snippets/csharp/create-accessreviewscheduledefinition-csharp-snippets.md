---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf0a43a55100fb7de8b8e68db09264ac3af48dfb
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753545"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = new AccessReviewScheduleDefinition
{
    DisplayName = "Test create",
    DescriptionForAdmins = "New scheduled access review",
    DescriptionForReviewers = "If you have any questions, contact jerry@contoso.com",
    Scope = new AccessReviewScope
    {
        Query = "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0c4444/transitiveMembers",
        QueryType = "MicrosoftGraph"
    },
    Reviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/users/7eae4444-d425-48b2-adf2-3c777f6256f3",
            QueryType = "MicrosoftGraph",
            QueryRoot = "decisions"
        }
    },
    Settings = new AccessReviewScheduleSettings
    {
        MailNotificationsEnabled = true,
        ReminderNotificationsEnabled = true,
        JustificationRequiredOnApproval = true,
        DefaultDecisionEnabled = false,
        DefaultDecision = "None",
        InstanceDurationInDays = 1,
        AutoApplyDecisionsEnabled = false,
        RecommendationsEnabled = true,
        Recurrence = new PatternedRecurrence
        {
            Pattern = new RecurrencePattern
            {
                Type = RecurrencePatternType.Weekly,
                Interval = 1
            },
            Range = new RecurrenceRange
            {
                Type = RecurrenceRangeType.NoEnd,
                StartDate = new Date(2020,9,8)
            }
        }
    }
};

await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .AddAsync(accessReviewScheduleDefinition);

```