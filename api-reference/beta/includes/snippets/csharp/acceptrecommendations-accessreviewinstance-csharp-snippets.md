---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: b7ab1bac61dd088cd2ca9b83f46f9e86ce36fc2e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.PendingAccessReviewInstances["70a68410-67f3-4d4c-b946-6989e050be19"]
    .AcceptRecommendations()
    .Request()
    .PostAsync();

```