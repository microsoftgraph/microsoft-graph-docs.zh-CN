---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94ba73f77aceb43d6a6bef60a72b3972c7946099
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688068"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = new AccessReviewScheduleDefinition
{
    Id = "60860cdd-fb4d-4054-91ba-f75e04444aa6",
    DisplayName = "Test world UPDATED NAME!",
    DescriptionForAdmins = "Test world",
    DescriptionForReviewers = "Test world",
    Scope = new AccessReviewQueryScope
    {
        Query = "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        QueryType = "MicrosoftGraph"
    },
    InstanceEnumerationScope = new AccessReviewQueryScope
    {
        Query = "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",
        QueryType = "MicrosoftGraph"
    },
    Reviewers = new List<AccessReviewReviewerScope>()
    {
    },
    Settings = new AccessReviewScheduleSettings
    {
        MailNotificationsEnabled = true,
        ReminderNotificationsEnabled = true,
        JustificationRequiredOnApproval = true,
        DefaultDecisionEnabled = false,
        DefaultDecision = "None",
        InstanceDurationInDays = 3,
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
                StartDate = new Date(2020,9,15)
            }
        }
    }
};

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"]
    .Request()
    .PutAsync(accessReviewScheduleDefinition);

```