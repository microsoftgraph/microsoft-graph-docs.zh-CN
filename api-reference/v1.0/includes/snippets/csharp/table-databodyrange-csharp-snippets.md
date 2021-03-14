---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d4bb4fd947f3298c216e5edee340fe32699e190
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806631"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .DataBodyRange()
    .Request()
    .GetAsync();

```