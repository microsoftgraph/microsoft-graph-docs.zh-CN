---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1d1976afe0b5424a2da058ef5b07eff436f1c9ee
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows
    .Request()
    .Skip(5)
    .Top(5)
    .GetAsync();

```