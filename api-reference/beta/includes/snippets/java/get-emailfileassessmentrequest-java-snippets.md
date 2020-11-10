---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e0d220a846aac5c81fe4c936eb2e0d512ee6220
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977855"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("ab2ad9b3-2213-4091-ae0c-08d76ddbcacf")
    .buildRequest()
    .get();

```