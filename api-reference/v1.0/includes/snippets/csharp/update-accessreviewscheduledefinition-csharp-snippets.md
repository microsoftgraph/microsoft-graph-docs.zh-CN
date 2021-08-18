---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac7f03f9fea426b643c09b56543b79cf1876d700
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = new AccessReviewScheduleDefinition
{
    Id = "60860cdd-fb4d-4054-91ba-f75e04444aa6",
    DisplayName = "Test world UPDATED NAME!",
    DescriptionForAdmins = "Test world",
    DescriptionForReviewers = "Test world",
    Scope = new AccessReviewScope
    {
        Query = "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        QueryType = "MicrosoftGraph"
    },
    InstanceEnumerationScope = new AccessReviewScope
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