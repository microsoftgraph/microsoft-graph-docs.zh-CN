---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf40a12cc004e35e9a6ed4a9d1abdccefaf690dcfcfc075c0d7517c6a4bc4b71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.ValueAxis
    .Request()
    .GetAsync();

```