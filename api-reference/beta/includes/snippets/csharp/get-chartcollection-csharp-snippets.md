---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f40fe1e21997ccaa1d575fe19d8fd32264d83380
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783349"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var charts = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts
    .Request()
    .GetAsync();

```