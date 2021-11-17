---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd49d4ba21ab9a87ad7e78125b07bb2c784a6ff340cb96fe4eb79df533532a6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesAgent = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Agents["{onPremisesAgent-id}"]
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```