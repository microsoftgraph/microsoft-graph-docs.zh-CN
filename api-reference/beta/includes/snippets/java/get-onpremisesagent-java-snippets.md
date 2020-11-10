---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f44d2119ab37262c479bdcefc238bd07b2285d76
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975654"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgent onPremisesAgent = graphClient.onPremisesPublishingProfiles("provisioning").agents("1234b780-965f-4149-85c5-a8c73e58b67d")
    .buildRequest()
    .expand("agentGroups")
    .get();

```