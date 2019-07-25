---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2c129dbb0dd445a746cab840ebf5eaf838ded49c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agentGroups = await graphClient.OnPremisesPublishingProfiles["provisioning"].AgentGroups
    .Request()
    .Expand("publishedResources")
    .GetAsync();

```