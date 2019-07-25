---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6c7071021404a5fbceabddf20271a5b31ebf39dd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866074"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .UsedRange(true)
    .Request()
    .GetAsync();

```