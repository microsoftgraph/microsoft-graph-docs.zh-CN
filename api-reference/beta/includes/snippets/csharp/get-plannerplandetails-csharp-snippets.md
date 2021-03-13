---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7eed5f0b5fcfb70ce417bdaf5d233d6918b0b5b9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlanDetails = await graphClient.Planner.Plans["{plannerPlan-id}"].Details
    .Request()
    .GetAsync();

```