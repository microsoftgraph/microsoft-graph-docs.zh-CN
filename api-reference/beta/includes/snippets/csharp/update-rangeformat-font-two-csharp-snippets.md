---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ef93d1bb29b7c7928fadf883745c0402ecd4dbec87ee6ddfc02744eff03b185
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Italic = true,
    Size = 26
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("$B$1").Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```