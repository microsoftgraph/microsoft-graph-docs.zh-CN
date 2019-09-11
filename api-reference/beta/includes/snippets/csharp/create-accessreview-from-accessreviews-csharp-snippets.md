---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 97ed2d2fa8aadb67b91d60283e52e243bc124b1c
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReview = new AccessReview
{
    DisplayName = "TestReview",
    StartDateTime = DateTimeOffset.Parse("2017-02-10T00:35:53.214Z"),
    EndDateTime = DateTimeOffset.Parse("2017-03-12T00:35:53.214Z"),
    ReviewedEntity = new Identity
    {
        Id = "99025615-a0b1-47ec-9117-35377b10998b"
    },
    ReviewerType = "delegated",
    BusinessFlowTemplateId = "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    Description = "Sample description",
    Reviewers = new List<AccessReviewReviewer>()
    {
        new AccessReviewReviewer
        {
            Id = "f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        new AccessReviewReviewer
        {
            Id = "5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    },
    Settings = new AccessReviewSettings
    {
        MailNotificationsEnabled = true,
        RemindersEnabled = true,
        JustificationRequiredOnApproval = true,
        AutoReviewEnabled = false,
        ActivityDurationInDays = 30,
        AutoApplyReviewResultsEnabled = false,
        AccessRecommendationsEnabled = false,
        RecurrenceSettings = new AccessReviewRecurrenceSettings
        {
            RecurrenceType = "onetime",
            RecurrenceEndType = "endBy",
            DurationInDays = 0,
            RecurrenceCount = 0
        },
        AutoReviewSettings = new AutoReviewSettings
        {
            NotReviewedResult = "Deny"
        }
    }
};

await graphClient.AccessReviews
    .Request()
    .AddAsync(accessReview);

```