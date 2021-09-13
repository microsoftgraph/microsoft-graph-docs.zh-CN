---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1af87ae21abd4e539da64d1a10f01a4ba888db9caa16e1e8ecb9a6bece526513
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106212"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookPivotTable = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables["{workbookPivotTable-id}"]
    .Request()
    .GetAsync();

```