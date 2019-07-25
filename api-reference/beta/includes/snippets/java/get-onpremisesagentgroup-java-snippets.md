---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0bf95d7cce61e2e7174a84f6f29360e05c451c1f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878554"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgentGroup onPremisesAgentGroup = graphClient.onPremisesPublishingProfiles("provisioning").agentGroups("2d55ed41-1619-4848-92bb-0576d3038682")
    .buildRequest()
    .expand("agents")
    .get();

```