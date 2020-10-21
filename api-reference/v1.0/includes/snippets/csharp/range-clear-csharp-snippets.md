---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc28759d2c021ee8556f06b9bdd5770c5ca91b95
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615737"
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