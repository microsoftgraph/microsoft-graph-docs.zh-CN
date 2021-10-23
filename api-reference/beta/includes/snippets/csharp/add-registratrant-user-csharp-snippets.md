---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5234857c9298be05057686570fc66e9d2555d7d
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistrant = new MeetingRegistrant
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
    .AddAsync(meetingRegistrant);

```