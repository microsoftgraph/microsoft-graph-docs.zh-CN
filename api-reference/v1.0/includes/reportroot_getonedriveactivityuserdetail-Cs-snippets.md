---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5ce449c1ff5eb0d1bf07b95d450aa36bca476c91
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOneDriveActivityUserDetail('D7')
    .Request()
    .GetAsync();

```