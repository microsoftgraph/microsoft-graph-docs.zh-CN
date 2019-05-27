---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 384141283eb8690b83cb3fde8db545bec2b56a44
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442751"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Unmerge()
    .Request()
    .PostAsync();

```