---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f8c925253bcabcc9e4299e6743f3981a4318a7e
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42815864"
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