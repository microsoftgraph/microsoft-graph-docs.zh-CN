---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dde114bee5cd909c82e0fd0ad2206c5039c97175
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882904"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsAfter(2)
    .Request()
    .GetAsync();

```