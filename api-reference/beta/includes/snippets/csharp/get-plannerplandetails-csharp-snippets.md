---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f40bd391c5cc96aa4e338544634f4ecc6c8afaf4b52209f31623f8649fbf837
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlanDetails = await graphClient.Planner.Plans["{plannerPlan-id}"].Details
    .Request()
    .GetAsync();

```