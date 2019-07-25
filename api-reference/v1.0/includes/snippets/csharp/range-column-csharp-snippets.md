---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a71ab851589bdd7d0259d5b521f22bddeb8363d4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857213"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Column(5)
    .Request()
    .GetAsync();

```