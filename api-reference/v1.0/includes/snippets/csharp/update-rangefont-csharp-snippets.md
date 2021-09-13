---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67df516e94be5a54dd4d90e287b6488406f7314442599f39925ac867f06b4608
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Bold = true,
    Color = "color-value",
    Italic = true,
    Name = "name-value",
    Size = 99,
    Underline = "underline-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```