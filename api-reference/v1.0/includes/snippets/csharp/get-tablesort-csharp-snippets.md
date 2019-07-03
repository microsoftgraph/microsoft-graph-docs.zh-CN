---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6f8380ff93709a01eec793180b5064684a36e935
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466847"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableSort = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Sort
    .Request()
    .GetAsync();

```