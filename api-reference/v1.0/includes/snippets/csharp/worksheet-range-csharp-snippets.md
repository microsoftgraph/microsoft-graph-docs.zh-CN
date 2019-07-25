---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a932615d11cc574f3b4cf0ccb24771f238ba10d1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884335"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .Range('A1:B2')
    .Request()
    .GetAsync();

```