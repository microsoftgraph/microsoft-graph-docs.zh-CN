---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d54207d72377c992708d0eb4d63703ef29363074
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var series = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Series
    .Request()
    .GetAsync();

```