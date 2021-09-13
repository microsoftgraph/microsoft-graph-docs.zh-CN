---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07698918c240ce7304833441354aa0a8cba8b8dd9d200667be387506004c91e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTable = new WorkbookTable
{
    Name = "name-value",
    ShowHeaders = true,
    ShowTotals = true,
    Style = "style-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .Request()
    .UpdateAsync(workbookTable);

```