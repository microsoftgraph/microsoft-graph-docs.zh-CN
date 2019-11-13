---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cd4529c0db6e1d261d9cd3e1f0d69d2438dcd26
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroup = await graphClient.Communications.Calls["{id}"].AudioRoutingGroups["{id}"]
    .Request()
    .GetAsync();

```