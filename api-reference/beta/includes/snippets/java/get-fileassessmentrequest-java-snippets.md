---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 587e41c8e6b489ccb298894a7eb0aaf558794e67
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977857"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("18406a56-7209-4720-a250-08d772fccdaa")
    .buildRequest()
    .get();

```