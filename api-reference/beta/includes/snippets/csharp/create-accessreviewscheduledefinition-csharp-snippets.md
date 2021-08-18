---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be037ca91a3b3e57b43a2c355e03d8dfb286acdf7ce9cc0209060d549f416f0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902620"
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