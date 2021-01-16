---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bff84bf168e3cea4b7300473749efd283af0540
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsBelow(2)
    .Request()
    .GetAsync();

```