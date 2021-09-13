---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7517b3481ccbdf3e4010764dbc4bc80160735bfee065178e9342ddf62c64c607
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104250"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pivotTables = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables
    .Request()
    .GetAsync();

```