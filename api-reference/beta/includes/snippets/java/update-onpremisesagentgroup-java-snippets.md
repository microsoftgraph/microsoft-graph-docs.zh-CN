---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99b29291914847f0a7c4034e891b2abb34ecaf88
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976904"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgentGroup onPremisesAgentGroup = new OnPremisesAgentGroup();
onPremisesAgentGroup.displayName = "Group New Name";

graphClient.onPremisesPublishingProfiles("provisioning").agentGroups("8832388F-3814-4952-B288-FFB62081FE25")
    .buildRequest()
    .patch(onPremisesAgentGroup);

```