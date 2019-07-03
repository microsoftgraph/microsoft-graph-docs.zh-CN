---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1b07201a333ece0b08679dbca4cc602c8d4c014d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500381"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .TotalRowRange()
    .Request()
    .PostAsync();

```