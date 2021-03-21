---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df7c1ce67ec930befcf8c10dec811c536f8e1b6e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963169"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var name = "test7";

var formula = "=SUM(Sheet2!$A$1+Sheet2!$A$2)";

var comment = "Comment for the named item";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names
    .AddFormulaLocal(name,formula,comment)
    .Request()
    .PostAsync();

```