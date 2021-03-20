---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cd4c6f57a2ce75e3415fb8beef996b42ff254a8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944107"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailFileAssessmentRequest threatAssessmentRequest = new EmailFileAssessmentRequest();
threatAssessmentRequest.recipientEmail = "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com";
threatAssessmentRequest.expectedAssessment = ThreatExpectedAssessment.BLOCK;
threatAssessmentRequest.category = ThreatCategory.MALWARE;
threatAssessmentRequest.contentData = "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC.....";

graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .post(threatAssessmentRequest);

```