---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 718c5013662f7edff1d9c61b6fbd2a8d0a654eb5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478991"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.Me.Onenote.Resources["{id}"]
    .Request()
    .Select( e => new {
             e.Content 
             })
    .GetAsync();

var content = resources.Content;

```