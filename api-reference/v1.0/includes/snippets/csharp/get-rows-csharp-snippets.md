---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c8d32a32facc21e62965a4ee196fbe1013906148
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740455"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].Range('A1:Z10').VisibleView().Rows
    .Request()
    .GetAsync();

```