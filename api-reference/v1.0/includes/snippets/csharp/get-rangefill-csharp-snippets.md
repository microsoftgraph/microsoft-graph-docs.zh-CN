---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5489dc5b30847d5009b909dc560db4aa8d52b73c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Fill
    .Request()
    .GetAsync();

```