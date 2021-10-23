---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3663f25b66f6c65945a1a2d0b0c6b5f564640dad
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561687"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistrant = new MeetingRegistrant
{
    FirstName = "Lisa",
    LastName = "Adkins",
    Email = "lisa.adkins@contoso.com",
    CustomQuestionAnswers = new List<CustomQuestionAnswer>()
    {
        new CustomQuestionAnswer
        {
            QuestionId = "MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=",
            Value = "No"
        },
        new CustomQuestionAnswer
        {
            QuestionId = "MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=",
            Value = "Internet"
        }
    }
};

await graphClient.Users["{user-id}"].OnlineMeetings["{onlineMeeting-id}"].Registration.Registrants
    .Request()
    .AddAsync(meetingRegistrant);

```