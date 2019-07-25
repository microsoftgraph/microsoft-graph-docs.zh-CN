---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 19aaa62f26007d0a1ae2e6ba64f8c04687305248
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723133"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .Range()
    .Request()
    .PostAsync();

```