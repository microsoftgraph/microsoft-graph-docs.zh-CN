---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e6ff6614270e98f19389d014d2fc02b94542a7e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807748"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agents = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Agents
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```