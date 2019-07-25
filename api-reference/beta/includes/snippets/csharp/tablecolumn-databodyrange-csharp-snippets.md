---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cd3a8bb10ab477afd9f19f7b7195794ca9a343dd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .DataBodyRange()
    .Request()
    .PostAsync();

```