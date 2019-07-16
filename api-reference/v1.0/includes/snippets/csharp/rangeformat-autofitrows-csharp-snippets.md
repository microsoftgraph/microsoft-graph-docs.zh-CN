---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1a79c9d5f0aeaa719f5871a4c1ed17f46790507f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format
    .AutofitRows()
    .Request()
    .PostAsync();

```