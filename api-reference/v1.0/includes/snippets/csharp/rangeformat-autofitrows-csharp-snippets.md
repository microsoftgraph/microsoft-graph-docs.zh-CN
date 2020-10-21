---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a79c9d5f0aeaa719f5871a4c1ed17f46790507f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611415"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format
    .AutofitRows()
    .Request()
    .PostAsync();

```