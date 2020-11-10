---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6e5afa39ce0caca66dd1874dd613be783490969
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952964"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailAssessmentRequest threatAssessmentRequest = new MailAssessmentRequest();
threatAssessmentRequest.recipientEmail = "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com";
threatAssessmentRequest.expectedAssessment = ThreatExpectedAssessment.BLOCK;
threatAssessmentRequest.category = ThreatCategory.SPAM;
threatAssessmentRequest.messageUri = "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=";

graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .post(threatAssessmentRequest);

```