---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 26df2f4b4f8c0d735c9015837350cdf88787c4b8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493523"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .HeaderRowRange()
    .Request()
    .PostAsync();

```