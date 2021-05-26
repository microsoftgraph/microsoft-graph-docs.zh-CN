---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bcba471d78bfe24d8941474bf6c89cdd5b0575a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664584"
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