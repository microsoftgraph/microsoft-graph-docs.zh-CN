---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 29e14f55a1676e2417668b8b201fc19184087694
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463762"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageUserDetail = await graphClient.Reports.GetTeamsDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```