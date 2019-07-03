---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 89124d7cc56bd84f3f4085dbe7caaf34a18ec934
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467089"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Range('A1:B2')
    .Request()
    .GetAsync();

```