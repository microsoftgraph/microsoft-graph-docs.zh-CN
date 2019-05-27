---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3dac820a91b45274c6798ceedb1c844f387b4e79
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447556"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Me.Planner.Plans
    .Request()
    .GetAsync();

```