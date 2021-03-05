---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 395161bc100268c7c701c3b17ae7d4eb07b0d710
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471722"
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
    Reviewers = new AccessReviewReviewersCollectionPage()
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