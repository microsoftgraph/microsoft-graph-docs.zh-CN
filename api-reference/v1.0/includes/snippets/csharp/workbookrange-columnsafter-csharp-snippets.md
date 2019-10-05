---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 20d5ce8d8c496c14c3dcd12e1312099f44f2bfd0
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsAfter(null)
    .Request()
    .PostAsync();

```