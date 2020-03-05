---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcec87234c0f12fa61d3c8701151b3d758f993f3
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parentReference = new ItemReference
{
    Id = "String"
};

var name = "String";

await graphClient.Me.Drive.Items["{item-id}"]
    .Restore(parentReference,name)
    .Request()
    .PostAsync();

```