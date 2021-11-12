---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1213e24f27f008e8314f024aacdd1b39ed5a0a85a1404705766e791bcc884c75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277379"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookWorksheet = new WorkbookWorksheet
{
    Position = 99,
    Name = "name-value",
    Visibility = "visibility-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Request()
    .UpdateAsync(workbookWorksheet);

```