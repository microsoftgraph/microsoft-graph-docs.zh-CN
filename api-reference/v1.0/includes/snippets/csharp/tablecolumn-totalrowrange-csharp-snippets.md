---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d524176d3bafc3f988f023d7bd1bce4542766098
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904577"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .TotalRowRange()
    .Request()
    .GetAsync();

```