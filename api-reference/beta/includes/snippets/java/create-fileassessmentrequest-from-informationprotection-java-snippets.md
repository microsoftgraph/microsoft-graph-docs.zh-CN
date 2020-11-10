---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f8c925253bcabcc9e4299e6743f3981a4318a7e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952968"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAssessmentRequest threatAssessmentRequest = new FileAssessmentRequest();
threatAssessmentRequest.expectedAssessment = ThreatExpectedAssessment.BLOCK;
threatAssessmentRequest.category = ThreatCategory.MALWARE;
threatAssessmentRequest.fileName = "test.txt";
threatAssessmentRequest.contentData = "VGhpcyBpcyBhIHRlc3QgZmlsZQ==";

graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .post(threatAssessmentRequest);

```