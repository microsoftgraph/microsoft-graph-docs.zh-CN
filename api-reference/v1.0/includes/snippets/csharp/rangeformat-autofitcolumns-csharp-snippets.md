---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 159dabac73c5c292e6473e76106fec4d0ec50f0b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738400"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format
    .AutofitColumns()
    .Request()
    .PostAsync();

```