---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 718c5013662f7edff1d9c61b6fbd2a8d0a654eb5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479148"
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