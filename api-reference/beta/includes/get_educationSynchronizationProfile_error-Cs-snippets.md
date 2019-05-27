---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1109d0b032d38cb7400ed5160f419dd4b98eed93
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var errors = await graphClient.Education.SynchronizationProfiles["{id}"].Errors
    .Request()
    .GetAsync();

```