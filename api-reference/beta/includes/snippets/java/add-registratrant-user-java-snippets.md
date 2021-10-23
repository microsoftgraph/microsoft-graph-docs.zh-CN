---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbaba310f9bffcfc53784242ff57e09c51ea9d67
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561729"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistrant meetingRegistrant = new MeetingRegistrant();
meetingRegistrant.firstName = "Frederick";
meetingRegistrant.lastName = "Cormier";
meetingRegistrant.email = "frederick.cormier@contoso.com";
LinkedList<CustomQuestionAnswer> customQuestionAnswersList = new LinkedList<CustomQuestionAnswer>();
CustomQuestionAnswer customQuestionAnswers = new CustomQuestionAnswer();
customQuestionAnswers.questionId = "MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=";
customQuestionAnswers.value = "No";
customQuestionAnswersList.add(customQuestionAnswers);
CustomQuestionAnswer customQuestionAnswers1 = new CustomQuestionAnswer();
customQuestionAnswers1.questionId = "MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=";
customQuestionAnswers1.value = "Internet";
customQuestionAnswersList.add(customQuestionAnswers1);
meetingRegistrant.customQuestionAnswers = customQuestionAnswersList;

graphClient.users("16664f75-11dc-4870-bec6-38c1aaa81431").onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().registrants()
    .buildRequest()
    .post(meetingRegistrant);

```