---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a99ce2d73c37bc4837fcb3049d84517a1f94767533483b233da2930e6bb61c9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocations = await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .Filter("isof('microsoft.graph.ipNamedLocation')")
    .GetAsync();

```