---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 60eb009f953fe4c7f7ce637cac6af05a4a4ee930
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Cell(5,6)
    .Request()
    .GetAsync();

```