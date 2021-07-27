---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eed78a6173e1b296ba557f16643de8daa238924
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581450"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var values = JsonDocument.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Add(null,values)
    .Request()
    .PostAsync();

```