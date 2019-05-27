---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7a7c230a0cc7fc35a607f5f2276e13e46cb91a02
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476898"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```