---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 921798615b104d5b58d55719acf59fd177efdba2
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = new AccessReviewScheduleDefinition
{
    DisplayName = "Test create",
    DescriptionForAdmins = "New scheduled access review",
    DescriptionForReviewers = "If you have any questions, contact jerry@contoso.com",
    Scope = new AccessReviewQueryScope
    {
        Query = "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers",
        QueryType = "MicrosoftGraph"
    },
    Reviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/users/398164b1-5196-49dd-ada2-364b49f99b27",
            QueryType = "MicrosoftGraph"
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