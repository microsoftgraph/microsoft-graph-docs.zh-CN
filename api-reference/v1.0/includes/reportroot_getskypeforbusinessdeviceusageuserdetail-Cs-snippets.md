---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2b470a435da2180dad2a3509ea091b78ecd7bba2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476884"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```