---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bea727a5f1590945ac48d9669e3527db0a3e78a1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].PublishedResources["{publishedResource-id}"].AgentGroups["{onPremisesAgentGroup-id}"].Reference
    .Request()
    .DeleteAsync();

```