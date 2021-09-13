---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3cd297f70113f565f5e4c7159c2759428b82c73cfa3ef7501eb58007df06f82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"]
    .DataBodyRange()
    .Request()
    .GetAsync();

```