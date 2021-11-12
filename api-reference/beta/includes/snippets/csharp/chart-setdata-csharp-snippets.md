---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b64adf3104b1f458835998f767dc226ca23cbab37be496cda84cd00ef12b6ec4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceData = JsonDocument.Parse(@"""sourceData-value""");

var seriesBy = "seriesBy-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"]
    .SetData(seriesBy,sourceData)
    .Request()
    .PostAsync();

```