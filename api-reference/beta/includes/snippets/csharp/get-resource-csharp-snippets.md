---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 718c5013662f7edff1d9c61b6fbd2a8d0a654eb5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718352"
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