---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 97f1735ba961191bb70da4c506c3af15c8027a8f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500395"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .TotalRowRange()
    .Request()
    .PostAsync();

```