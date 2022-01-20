---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4db09bbb2aa9f1bb7fe8ec47b16147089a172c65
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137655"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistrant meetingRegistrantBase = new MeetingRegistrant();
meetingRegistrantBase.firstName = "Frederick";
meetingRegistrantBase.lastName = "Cormier";
meetingRegistrantBase.email = "frederick.cormier@contoso.com";
LinkedList<CustomQuestionAnswer> customQuestionAnswersList = new LinkedList<CustomQuestionAnswer>();
CustomQuestionAnswer customQuestionAnswers = new CustomQuestionAnswer();
customQuestionAnswers.questionId = "MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=";
customQuestionAnswers.value = "No";
customQuestionAnswersList.add(customQuestionAnswers);
CustomQuestionAnswer customQuestionAnswers1 = new CustomQuestionAnswer();
customQuestionAnswers1.questionId = "MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=";
customQuestionAnswers1.value = "Internet";
customQuestionAnswersList.add(customQuestionAnswers1);
meetingRegistrantBase.customQuestionAnswers = customQuestionAnswersList;

graphClient.users("16664f75-11dc-4870-bec6-38c1aaa81431").onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().registrants()
    .buildRequest()
    .post(meetingRegistrantBase);

```