---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e7a2f4f67e9f05321fd2d2047504810c569b1e6f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500483"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartPoint = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series["{undefined}"].Points["{undefined}"]
    .Request()
    .GetAsync();

```