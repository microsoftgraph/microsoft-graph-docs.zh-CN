---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3a055457da12e3abbe2bf91eeda1f6e01c58c87
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779895"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .TotalRowRange()
    .Request()
    .GetAsync();

```