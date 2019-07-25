---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3dac820a91b45274c6798ceedb1c844f387b4e79
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730124"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Me.Planner.Plans
    .Request()
    .GetAsync();

```