---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9780c7bef263a08a3835f96f75d7c586399dc7de
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "edit";

var scope = "organization";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,scope,null,null,null,null)
    .Request()
    .PostAsync();

```