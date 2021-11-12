---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4872d5db7d4fa4b35e269113a7bcc46eba7ed7df5a0e97b7401e9b6f5f4ac7e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartGridlines = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.ValueAxis.MinorGridlines
    .Request()
    .GetAsync();

```