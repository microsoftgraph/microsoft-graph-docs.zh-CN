---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2878356faa7d8e8fc79dd2dffd524a8bb80f7464
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Protection
    .Request()
    .GetAsync();

```