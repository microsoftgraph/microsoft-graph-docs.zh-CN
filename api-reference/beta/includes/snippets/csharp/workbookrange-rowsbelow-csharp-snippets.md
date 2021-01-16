---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1819d1be7ccd31f99b51bffc8afa7d428869af06
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsBelow(2)
    .Request()
    .GetAsync();

```