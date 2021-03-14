---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10992f84ef015eff6d32f2597e08a12102ed5a86
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Plans["{plannerPlan-id}"].Buckets
    .Request()
    .GetAsync();

```