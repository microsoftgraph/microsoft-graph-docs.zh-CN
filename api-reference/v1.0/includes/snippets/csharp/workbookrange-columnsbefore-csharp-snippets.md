---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d0c4e9fd6dd69d7b9e0c62012fecc8b26c520a85
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsBefore(null)
    .Request()
    .PostAsync();

```