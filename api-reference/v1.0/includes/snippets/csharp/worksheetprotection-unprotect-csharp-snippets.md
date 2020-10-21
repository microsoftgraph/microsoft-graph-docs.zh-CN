---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72520adae193e0ab3182c33c1b438e3a8986454f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618761"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var password = "password-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
    .Unprotect()
    .Request()
    .PostAsync();

```