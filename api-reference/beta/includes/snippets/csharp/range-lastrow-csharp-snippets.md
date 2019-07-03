---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5c54f47215b0dcfd595790cf1d612455c09d6c2c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479458"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().LastRow()
    .Request()
    .GetAsync();

```