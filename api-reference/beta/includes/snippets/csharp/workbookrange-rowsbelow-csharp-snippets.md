---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c58224e5526d0b829237f782c169dfd0c1c7e0f3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716054"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsBelow(count)
    .Request()
    .PostAsync();

```