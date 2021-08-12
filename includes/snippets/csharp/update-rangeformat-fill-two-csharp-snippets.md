---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f198ec03f3aa3bd21f088987f1112eddb905ce33184d0242bf0df5ce5ed33b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237707"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#00FF00"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range("$B$1").Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```