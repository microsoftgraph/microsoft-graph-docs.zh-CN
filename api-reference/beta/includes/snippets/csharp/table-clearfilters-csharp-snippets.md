---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e64bac722ba797220ed4998ece71ff952bebcc78
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717274"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ClearFilters()
    .Request()
    .PostAsync();

```