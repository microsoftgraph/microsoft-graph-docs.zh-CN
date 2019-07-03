---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 37094b84a729121d73dd88fe8ce6bb07f59abb44
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var charts = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts
    .Request()
    .GetAsync();

```