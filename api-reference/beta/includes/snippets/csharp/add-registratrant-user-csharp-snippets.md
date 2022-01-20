---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 694611c29789bbdac9bc47bfc19816236fd23a19
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistrantBase = new MeetingRegistrant
{
    FirstName = "Frederick",
    LastName = "Cormier",
    Email = "frederick.cormier@contoso.com",
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