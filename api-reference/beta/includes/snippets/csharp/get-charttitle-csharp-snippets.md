---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f3530b6c55226fb30f45ccc8fcdeb61dea5d9773e39c542d274a9eb5855c0ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartTitle = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Title
    .Request()
    .GetAsync();

```