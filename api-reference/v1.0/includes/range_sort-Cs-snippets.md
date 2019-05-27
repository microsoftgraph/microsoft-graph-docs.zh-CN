---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1d11751ef93790d7a3f1c160e673a27441f14121
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453854"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeSort = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Sort
    .Request()
    .GetAsync();

```