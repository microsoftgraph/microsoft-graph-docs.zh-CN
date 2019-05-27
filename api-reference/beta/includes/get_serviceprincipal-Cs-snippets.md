---
description: 自动生成的文件。 不修改
ms.openlocfilehash: da3483616be48434ac83dc126a7bdda639dc5205
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = await graphClient.ServicePrincipals["{id}"]
    .Request()
    .GetAsync();

```