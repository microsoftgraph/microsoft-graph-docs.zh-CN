---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4632d0397d125340bbe74d4fdb0a10d6e1f08d09
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402408"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsAfter(null)
    .Request()
    .PostAsync();

```