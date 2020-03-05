---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7024a2bc21af591064697f77d5c1b5c67cb5e673
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Updating the latest guidelines";

await graphClient.Drives["{drive-id}"].Items["{item-id}"]
    .Checkin(null,comment)
    .Request()
    .PostAsync();

```