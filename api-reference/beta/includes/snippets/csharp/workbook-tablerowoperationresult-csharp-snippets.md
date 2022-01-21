---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f899fc902d75b2d95837f3c0e69fa1259a22bce
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableRow = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook
    .TableRowOperationResult("0195cfac-bd22-4f91-b276-dece0aa2378b")
    .Request()
    .GetAsync();

```