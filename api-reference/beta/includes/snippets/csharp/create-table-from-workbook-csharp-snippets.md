---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3915431da2b96744e40e0db1618f26ccfb803d5b
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402569"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "A1:D8";

var hasHeaders = false;

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables
    .Add(hasHeaders,address)
    .Request()
    .PostAsync();

```