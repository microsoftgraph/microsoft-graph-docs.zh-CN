---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eadd2a3fe1b6b03d1c2944e9674a734f2091ea47
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522723"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = await graphClient.DirectoryRoles["23f3b4b4-8a29-4420-8052-e4950273bbda"]
    .Request()
    .GetAsync();

```