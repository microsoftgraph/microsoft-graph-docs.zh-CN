---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61fbd62e4afb8a28244a8e81ac38bc29b72c56b3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var accessReviewScheduleDefinition = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"{
  ""id"": ""60860cdd-fb4d-4054-91ba-f75e04444aa6"",
  ""displayName"": ""Test world UPDATED NAME!"",
  ""descriptionForAdmins"": ""Test world"",
  ""descriptionForReviewers"": ""Test world"",
  ""scope"": {
    ""query"": ""/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers"",
    ""queryType"": ""MicrosoftGraph""
  },
  ""instanceEnumerationScope"": {
    ""query"": ""/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f"",
    ""queryType"": ""MicrosoftGraph""
  },
  ""reviewers"": [],
  ""settings"": {
    ""mailNotificationsEnabled"": true,
    ""reminderNotificationsEnabled"": true,
    ""justificationRequiredOnApproval"": true,
    ""defaultDecisionEnabled"": false,
    ""defaultDecision"": ""None"",
    ""instanceDurationInDays"": 3,
    ""autoApplyDecisionsEnabled"": false,
    ""recommendationsEnabled"": true,
    ""recurrence"": {
      ""pattern"": {
        ""type"": ""weekly"",
        ""interval"": 1
      },
      ""range"": {
        ""type"": ""noEnd"",
        ""startDate"": ""2020-09-15""
      }
    }
  }
}"));

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"]
    .Request()
    .PutAsync(accessReviewScheduleDefinition);

```