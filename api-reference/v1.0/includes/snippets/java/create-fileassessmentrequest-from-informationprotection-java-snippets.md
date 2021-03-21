---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99335696ed5b0e79218dc85edb6dd0a95a524d00
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956532"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAssessmentRequest threatAssessmentRequest = new FileAssessmentRequest();
threatAssessmentRequest.expectedAssessment = ThreatExpectedAssessment.BLOCK;
threatAssessmentRequest.category = ThreatCategory.MALWARE;
threatAssessmentRequest.fileName = "test.txt";
threatAssessmentRequest.contentData = "VGhpcyBpcyBhIHRlc3QgZmlsZQ==";

graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .post(threatAssessmentRequest);

```