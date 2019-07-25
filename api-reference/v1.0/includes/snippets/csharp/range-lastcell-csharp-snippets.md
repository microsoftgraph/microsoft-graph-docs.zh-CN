---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d3937f0e4850a2849884c1f03bfe479deae5a40
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891278"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .LastCell()
    .Request()
    .GetAsync();

```