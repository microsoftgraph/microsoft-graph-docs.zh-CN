---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9777e24d2d45e6b613ed81b94259fc8c6217b538
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pivotTables = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].PivotTables
    .Request()
    .GetAsync();

```