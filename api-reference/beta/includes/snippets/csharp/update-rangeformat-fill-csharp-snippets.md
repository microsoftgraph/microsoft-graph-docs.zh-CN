---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc7a11b70b22950c60f6a106c066739424dffb98baa8bc252c903eb93427f3df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903746"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#FF0000"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("$A$1").Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```