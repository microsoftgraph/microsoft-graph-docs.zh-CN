---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fa6d52a7e47af12dc72fbb8849ea8d2d93121c7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pivotTables = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables
    .Request()
    .GetAsync();

```