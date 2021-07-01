---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c9567be12038da64c43e0707bd496b2f00adc03
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var definitions = await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```