---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06f7ded477abc71ab766b6e95a75c7888e574a72
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977853"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("723c35be-8b5a-47ae-29c0-08d76ddb7f5b")
    .buildRequest()
    .get();

```