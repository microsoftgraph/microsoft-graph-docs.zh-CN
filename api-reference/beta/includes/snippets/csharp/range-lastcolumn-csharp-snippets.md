---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 15629f91eff7a235e398c068d1f8be0b60300c3c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479459"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().LastColumn()
    .Request()
    .GetAsync();

```