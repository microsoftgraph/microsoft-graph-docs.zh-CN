---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 183c5c493e2eebb79dafb2c25fb6f7bb524caa9a
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559143"
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