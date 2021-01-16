---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcdeca02d667849c32bfc675d6c6277c66f7f3ff
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882945"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsAbove(2)
    .Request()
    .GetAsync();

```