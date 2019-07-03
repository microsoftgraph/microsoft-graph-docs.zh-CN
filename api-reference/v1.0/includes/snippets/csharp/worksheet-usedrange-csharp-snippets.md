---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8a2e624a82fd1e3c7fe9eedbbf2250a8da2f1bba
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510059"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].UsedRange()
    .Request()
    .GetAsync();

```