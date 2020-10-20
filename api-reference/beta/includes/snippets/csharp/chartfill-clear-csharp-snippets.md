---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93f29fa2451441f78b5776b0a9ee831de27a8126
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620126"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Format.Fill
    .Clear()
    .Request()
    .PostAsync();

```