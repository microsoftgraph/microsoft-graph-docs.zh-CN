---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 664cc681c35211f6b017012b409d778d510e4a2b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137658"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistrantBase = new MeetingRegistrant
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
    .AddAsync(meetingRegistrantBase);

```