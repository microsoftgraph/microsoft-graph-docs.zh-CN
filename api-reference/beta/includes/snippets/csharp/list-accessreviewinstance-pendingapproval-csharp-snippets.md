---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a608feffe462b04970ec24cd590e048fb6b33b5b2e0492eae8eea2eab59b265
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902673"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pendingAccessReviewInstances = await graphClient.Me.PendingAccessReviewInstances
    .Request()
    .Expand("definition")
    .Skip(0)
    .Top(100)
    .GetAsync();

```