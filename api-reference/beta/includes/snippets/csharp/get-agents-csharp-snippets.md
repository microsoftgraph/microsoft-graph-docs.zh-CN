---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 27237b7467100b49453b35c7f2b76b90560570b6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agents = await graphClient.OnPremisesPublishingProfiles["provisioning"].Agents
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```