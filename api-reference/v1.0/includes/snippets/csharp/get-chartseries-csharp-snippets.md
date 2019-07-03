---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7d0f2258e5d155cb2ba309bd5e359a54eae51274
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467545"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartSeries = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series["{series-id}"]
    .Request()
    .GetAsync();

```