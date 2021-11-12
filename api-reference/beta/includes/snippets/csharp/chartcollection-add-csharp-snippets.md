---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fbea60302dbb54cd9a2bafff464a724bd8014ebb14faf16b6f03f7ce88d6db4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "ColumnStacked";

var sourceData = JsonDocument.Parse(@"""A1:B1""");

var seriesBy = "Auto";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts
    .Add(type,seriesBy,sourceData)
    .Request()
    .PostAsync();

```