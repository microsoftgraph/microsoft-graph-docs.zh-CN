---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e270fece51cc9807a6b4271bd8f8d6e61aa549d205159205846b24d3d5309792
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219271"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChart = new WorkbookChart
{
    Height = 99,
    Left = 99
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"]
    .Request()
    .UpdateAsync(workbookChart);

```