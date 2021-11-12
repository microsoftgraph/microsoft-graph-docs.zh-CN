---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 459bfc498b9a3d0b7c4a77b31663eedf374f9f5a9e6b6179b60b7932fcd40722
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219788"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var points = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Series["{workbookChartSeries-id}"].Points
    .Request()
    .GetAsync();

```