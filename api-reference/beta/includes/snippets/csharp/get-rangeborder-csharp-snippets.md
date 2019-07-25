---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 622556fc3a161743c40dbbe040b357b6e1d1c2be
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874645"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeBorder = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Borders["{sideIndex}"]
    .Request()
    .GetAsync();

```