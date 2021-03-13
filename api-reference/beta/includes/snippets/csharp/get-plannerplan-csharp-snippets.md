---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a741b759a4deb42eb6bad3f314b6294eb28ebcc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780875"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = await graphClient.Planner.Plans["{plannerPlan-id}"]
    .Request()
    .GetAsync();

```