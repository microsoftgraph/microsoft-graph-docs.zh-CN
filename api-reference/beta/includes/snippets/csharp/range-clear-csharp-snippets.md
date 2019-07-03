---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bc28759d2c021ee8556f06b9bdd5770c5ca91b95
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applyTo = "applyTo-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Clear(applyTo)
    .Request()
    .PostAsync();

```