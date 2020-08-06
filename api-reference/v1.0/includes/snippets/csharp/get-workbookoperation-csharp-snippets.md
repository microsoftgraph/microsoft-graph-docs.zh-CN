---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b49d773000d560ba2677fdb3b3417f26e5528a21
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookOperation = await graphClient.Me.Drive.Items["{drive-item-id}"].Workbook.Operations["{operation-id}"]
    .Request()
    .GetAsync();

```