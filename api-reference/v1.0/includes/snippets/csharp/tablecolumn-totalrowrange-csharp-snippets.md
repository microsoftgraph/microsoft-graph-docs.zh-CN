---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 032ce0576f2e18beda115c001295aac968ec9cc60e08ba88a4b162c52e575834
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"]
    .TotalRowRange()
    .Request()
    .GetAsync();

```