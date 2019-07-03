---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1133eb04cad418ff106abfc4c238337eddc851bd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520146"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsAbove(count)
    .Request()
    .PostAsync();

```