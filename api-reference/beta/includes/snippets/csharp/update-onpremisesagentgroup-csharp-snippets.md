---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 963f0d8b12dc9c70f14d9afbde2f2a38eb758d51
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesAgentGroup = new OnPremisesAgentGroup
{
    DisplayName = "Group New Name"
};

await graphClient.OnPremisesPublishingProfiles["provisioning"].AgentGroups["8832388F-3814-4952-B288-FFB62081FE25"]
    .Request()
    .UpdateAsync(onPremisesAgentGroup);

```