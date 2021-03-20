---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 258c6a164a1dacf8053e499c663f189874ec2158
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocations = await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .Filter("isof('microsoft.graph.ipNamedLocation')")
    .GetAsync();

```