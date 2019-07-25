---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f44d2119ab37262c479bdcefc238bd07b2285d76
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878722"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgent onPremisesAgent = graphClient.onPremisesPublishingProfiles("provisioning").agents("1234b780-965f-4149-85c5-a8c73e58b67d")
    .buildRequest()
    .expand("agentGroups")
    .get();

```