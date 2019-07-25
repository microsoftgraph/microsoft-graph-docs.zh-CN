---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1fc42477bcb909ca1632fea105668e44939b547d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878721"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesAgent = await graphClient.OnPremisesPublishingProfiles["provisioning"].Agents["1234b780-965f-4149-85c5-a8c73e58b67d"]
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```