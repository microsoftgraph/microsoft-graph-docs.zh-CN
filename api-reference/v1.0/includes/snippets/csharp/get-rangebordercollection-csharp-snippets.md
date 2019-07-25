---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4aeb43531a8836468a7ccb72741ed5761e5a725f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var borders = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Borders
    .Request()
    .GetAsync();

```