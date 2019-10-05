---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bea8813c466f9afd1a18b989c18dd0fa61c7ae12
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites
    .Request()
    .Filter("siteCollection/root ne null")
    .Select( e => new {
             e.SiteCollection,
             e.WebUrl 
             })
    .GetAsync();

```