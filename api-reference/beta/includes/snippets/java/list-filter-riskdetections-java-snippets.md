---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 595a3d3ec94b9c772b0304598009cb96a6561042
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977689"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRiskDetectionCollectionPage riskDetections = graphClient.identityProtection().riskDetections()
    .buildRequest()
    .filter("riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'")
    .get();

```