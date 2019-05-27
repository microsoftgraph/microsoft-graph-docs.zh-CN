---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 653e39f552c1009bcf1de614cc85d97041e3bb18
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480293"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRooms = await graphClient.Me.FindRooms('Building2Rooms@contoso.onmicrosoft.com')
    .Request()
    .GetAsync();

```