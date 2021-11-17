---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf38c6db2ec1eb0b47b0594f25858ece375fb56cc85f9e6aa1106affb1c8e44e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161426"
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