---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef7d4385932ee3b92cf7262e841a93b93ddb09ce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797895"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decisions = await graphClient.Me.PendingAccessReviewInstances["{accessReviewInstance-id}"].Decisions
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```