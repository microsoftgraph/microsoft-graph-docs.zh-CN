---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8465f1f02fe9e586257ea4558f2352d967762f67
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302860"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{id}"].AudioRoutingGroups["{id}"]
    .Request()
    .DeleteAsync();

```