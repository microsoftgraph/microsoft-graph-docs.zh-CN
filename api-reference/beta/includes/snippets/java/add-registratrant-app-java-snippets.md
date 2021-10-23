---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aad7db12319b953bf437e814940e22da57d4c771
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561722"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistrant meetingRegistrant = new MeetingRegistrant();
meetingRegistrant.firstName = "Lisa";
meetingRegistrant.lastName = "Adkins";
meetingRegistrant.email = "lisa.adkins@contoso.com";
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

graphClient.users("dc17674c-81d9-4adb-bfb2-8f6a442e4622").onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().registrants()
    .buildRequest()
    .post(meetingRegistrant);

```