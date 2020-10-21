---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e64bac722ba797220ed4998ece71ff952bebcc78
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ClearFilters()
    .Request()
    .PostAsync();

```