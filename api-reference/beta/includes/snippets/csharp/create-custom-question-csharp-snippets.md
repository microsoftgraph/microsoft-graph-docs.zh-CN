---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 183c5c493e2eebb79dafb2c25fb6f7bb524caa9a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistrationQuestion = new MeetingRegistrationQuestion
{
    DisplayName = "What's your job position?",
    IsRequired = false,
    AnswerInputType = AnswerInputType.Text
};

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.CustomQuestions
    .Request()
    .AddAsync(meetingRegistrationQuestion);

```