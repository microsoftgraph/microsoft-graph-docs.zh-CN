---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4c5c3a6d0fd0fac133e89dc051e09a6c1eb74967
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723053"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .HeaderRowRange()
    .Request()
    .PostAsync();

```