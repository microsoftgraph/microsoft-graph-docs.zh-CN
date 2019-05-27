---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bb4877f494f4bd4f9620268232baa74d70474948
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454487"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedTimeZones = await graphClient.Me.Outlook.SupportedTimeZones()
    .Request()
    .GetAsync();

```