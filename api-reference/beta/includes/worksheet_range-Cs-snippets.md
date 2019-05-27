---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c6e58cd786b2cbf40045c728a13a0f63dfe47344
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453150"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "address-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .Range()
    .Request()
    .PostAsync();

```