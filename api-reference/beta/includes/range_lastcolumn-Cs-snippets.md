---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 15629f91eff7a235e398c068d1f8be0b60300c3c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442835"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().LastColumn()
    .Request()
    .GetAsync();

```