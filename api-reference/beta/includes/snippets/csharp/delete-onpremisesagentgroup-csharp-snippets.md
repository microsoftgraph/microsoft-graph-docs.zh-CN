---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d6de3133fc1362066f5cb67027b017eb0e8aba5d042943da3cf409989dfb263
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].AgentGroups["{onPremisesAgentGroup-id}"]
    .Request()
    .DeleteAsync();

```