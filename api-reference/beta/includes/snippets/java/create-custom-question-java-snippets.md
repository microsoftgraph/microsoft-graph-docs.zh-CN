---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92e691919db6ceed91f407211474cb796912587f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105886"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistrationQuestion meetingRegistrationQuestion = new MeetingRegistrationQuestion();
meetingRegistrationQuestion.displayName = "What's your job position?";
meetingRegistrationQuestion.isRequired = false;
meetingRegistrationQuestion.answerInputType = AnswerInputType.TEXT;

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().microsoft.graph.meetingRegistration().customQuestions()
    .buildRequest()
    .post(meetingRegistrationQuestion);

```