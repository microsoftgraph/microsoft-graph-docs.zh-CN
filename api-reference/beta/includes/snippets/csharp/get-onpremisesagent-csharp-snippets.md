---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 159ac349d4ac2c789f30fef4c4d74779e3a18593
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787520"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesAgent = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Agents["{onPremisesAgent-id}"]
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```