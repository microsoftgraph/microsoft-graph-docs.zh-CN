---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16bdbb0dd2d7ee3e5c0cc35e65e05ed00499d29b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604796"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Request()
    .PostAsync();

```