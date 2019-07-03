---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ec1e3b02899db809f8d4a8a14d1623f1e19f0593
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var across = true;

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Merge(across)
    .Request()
    .PostAsync();

```