---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b647a50659bb2e239c1306d2d3a65adbbe2feed6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477059"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointSiteUsagePages('D7')
    .Request()
    .GetAsync();

```