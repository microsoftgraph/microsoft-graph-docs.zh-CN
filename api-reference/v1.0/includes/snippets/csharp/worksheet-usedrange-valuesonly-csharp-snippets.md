---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7eac7b67ba95b479d3894e587eaa361225b8260d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].UsedRange(true)
    .Request()
    .GetAsync();

```