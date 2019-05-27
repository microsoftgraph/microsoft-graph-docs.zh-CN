---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c5228e0b6564275c386b8efe3cd1eb79a7a0e7de
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageUserCounts = await graphClient.Reports.GetTeamsDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```