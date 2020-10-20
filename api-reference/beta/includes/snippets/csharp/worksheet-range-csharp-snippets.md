---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6e58cd786b2cbf40045c728a13a0f63dfe47344
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "address-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .Range()
    .Request()
    .PostAsync();

```