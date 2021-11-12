---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1433cd082987ff416c9abdb5696d36014b55a471839cfdab2711d8ea7f1dd163
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartFont = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.ValueAxis.Format.Font
    .Request()
    .GetAsync();

```