---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7fbca8d812c087ee9e6603259e8c3aa6d1b459a1
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402837"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsBelow(null)
    .Request()
    .PostAsync();

```