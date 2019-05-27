---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 762704527d002291e1012a30651f7712933a0977
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnits = await graphClient.AdministrativeUnits
    .Request()
    .GetAsync();

```