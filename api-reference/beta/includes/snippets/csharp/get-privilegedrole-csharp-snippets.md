---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05fde81ae3f898f10066cf0d2f2427357d1352ab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRole = await graphClient.PrivilegedRoles["{privilegedRole-id}"]
    .Request()
    .GetAsync();

```