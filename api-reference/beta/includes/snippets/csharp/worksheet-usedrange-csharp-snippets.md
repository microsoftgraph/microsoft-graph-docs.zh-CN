---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51ced96f9c9f9010a3eb6a97358c3586a7cc4bfe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795837"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .UsedRange(true)
    .Request()
    .GetAsync();

```