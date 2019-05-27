---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 81cb511d07cb9f8079cc625eb4aab928c0ff0c6e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474196"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreements = await graphClient.Agreements
    .Request()
    .GetAsync();

```