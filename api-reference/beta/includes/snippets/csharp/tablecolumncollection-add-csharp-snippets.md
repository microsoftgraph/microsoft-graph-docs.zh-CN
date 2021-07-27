---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b7f9e084f8e8739d6ee8b1e4dfb5462cdd84e24
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581302"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = new Int32
{
};

var values = JsonDocument.Parse("[{}]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns
    .Add(index,values,null)
    .Request()
    .PostAsync();

```