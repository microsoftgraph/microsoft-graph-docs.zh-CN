---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fec7262a430de0a0f4208d46bf135c283ecf4c8c
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806748"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"].TokenLifetimePolicies["{id}"].Reference
    .Request()
    .DeleteAsync();

```