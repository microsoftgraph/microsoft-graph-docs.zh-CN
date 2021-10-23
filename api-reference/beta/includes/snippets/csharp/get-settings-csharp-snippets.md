---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1a8f80866d2d81b3d3a188231d42ebd0c8542d5
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559879"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var caseSettings = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Settings
    .Request()
    .GetAsync();

```