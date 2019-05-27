---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ab8dd3fdcb386d6c07833cd97144c59f5144f2ba
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().EntireColumn()
    .Request()
    .GetAsync();

```