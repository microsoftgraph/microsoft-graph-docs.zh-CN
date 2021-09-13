---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac8e75e8e0c26263bc0c84f049fd33944023b0f6884fdf0bdb55f58229e6b300
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.SeriesAxis.Format.Line
    .Clear()
    .Request()
    .PostAsync();

```