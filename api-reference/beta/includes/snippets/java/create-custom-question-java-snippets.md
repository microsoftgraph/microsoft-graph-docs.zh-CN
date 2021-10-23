---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7522fa00750f2e6ce3e3f6cb96ef538d606784a2
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559139"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistrationQuestion meetingRegistrationQuestion = new MeetingRegistrationQuestion();
meetingRegistrationQuestion.displayName = "What's your job position?";
meetingRegistrationQuestion.isRequired = false;
meetingRegistrationQuestion.answerInputType = AnswerInputType.TEXT;

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().customQuestions()
    .buildRequest()
    .post(meetingRegistrationQuestion);

```