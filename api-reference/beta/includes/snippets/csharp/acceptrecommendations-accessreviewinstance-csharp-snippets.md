---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cf37c053d68545b0e5e5e6c784b43ac36099d13
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.PendingAccessReviewInstances["{accessReviewInstance-id}"]
    .AcceptRecommendations()
    .Request()
    .PostAsync();

```