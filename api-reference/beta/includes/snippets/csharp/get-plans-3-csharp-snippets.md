---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1748ad711fdb82d27d3b917e64f4bfe67b4975012c24141438f3125c895222c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328860"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Me.Planner.Plans
    .Request()
    .GetAsync();

```