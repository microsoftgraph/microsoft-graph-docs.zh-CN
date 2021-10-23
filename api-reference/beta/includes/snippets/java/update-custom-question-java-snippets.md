---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f983f5d1461981788fc48dc4740c5a789a5fbd7d
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558608"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistrationQuestion meetingRegistrationQuestion = new MeetingRegistrationQuestion();
meetingRegistrationQuestion.answerInputType = AnswerInputType.RADIO_BUTTON;
LinkedList<String> answerOptionsList = new LinkedList<String>();
answerOptionsList.add("Software Engineer");
answerOptionsList.add("Software Development Manager");
answerOptionsList.add("Product Manager");
answerOptionsList.add("Data scientist");
answerOptionsList.add("Other");
meetingRegistrationQuestion.answerOptions = answerOptionsList;

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().customQuestions("MSNhYjc5NWI4MC119zX3gwMDIwX3lvdXJfeDAwMjBfam8=")
    .buildRequest()
    .patch(meetingRegistrationQuestion);

```