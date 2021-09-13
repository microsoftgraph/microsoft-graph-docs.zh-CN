---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f74ed47e58aea5398d1cd3b8ddcb6b9a3087731ab889532da79afa5dae5bac2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChart = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"]
    .Request()
    .GetAsync();

```