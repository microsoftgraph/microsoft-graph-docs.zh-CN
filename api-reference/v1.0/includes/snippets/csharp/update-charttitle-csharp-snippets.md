---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4b72bb195be7931e74ba56ea2020e764236e277ee2c804afe814b4dbae02472
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378456"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartTitle = new WorkbookChartTitle
{
    Overlay = true,
    Text = "text-value",
    Visible = true
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Title
    .Request()
    .UpdateAsync(workbookChartTitle);

```