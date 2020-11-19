---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 3c9567be12038da64c43e0707bd496b2f00adc03
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214218"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var definitions = await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```