---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a106516f631737c5482e7cd76b1aeae59faa2dae27b6997ff6a75abaced8b9a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var charts = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts
    .Request()
    .GetAsync();

```