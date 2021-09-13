---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06aedca97312f1f372a814abbc917a05188f9d49f2c39273a2d32f334ba58462
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378794"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var color = "color-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Format.Fill
    .SetSolidColor(color)
    .Request()
    .PostAsync();

```