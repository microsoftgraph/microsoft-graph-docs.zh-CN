---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e144424c2e7af2107536ceda2d25445c2506961
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsBefore(2)
    .Request()
    .GetAsync();

```