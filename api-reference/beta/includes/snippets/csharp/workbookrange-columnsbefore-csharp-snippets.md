---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09600b6fed28f0808cf8158bee708788c43bca35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806584"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .ColumnsBefore(2)
    .Request()
    .GetAsync();

```