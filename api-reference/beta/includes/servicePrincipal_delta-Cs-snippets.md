---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c038417fcc79621c6a19fdd10cb65b761a45dc8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.ServicePrincipals.Delta()
    .Request()
    .GetAsync();

```