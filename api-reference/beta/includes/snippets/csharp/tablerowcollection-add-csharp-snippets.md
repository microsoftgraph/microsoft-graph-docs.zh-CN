---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 7280b9ac52aac596aaff55ee63e3bde35796fd81
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/11/2020
ms.locfileid: "48994524"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

Int32? index = null;

var values = JToken.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows
    .Add(index,values)
    .Request()
    .PostAsync();

```