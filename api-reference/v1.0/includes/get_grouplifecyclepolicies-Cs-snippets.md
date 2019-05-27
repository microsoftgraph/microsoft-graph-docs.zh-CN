---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6deea81809038243dba78fcaae14a82900e00dd4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicies = await graphClient.Groups["{id}"].GroupLifecyclePolicies
    .Request()
    .GetAsync();

```