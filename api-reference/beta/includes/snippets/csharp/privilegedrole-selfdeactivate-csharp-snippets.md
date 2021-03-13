---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3de51d2092a34d8dab737fb0e1b66aa18f10b4b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoles["{privilegedRole-id}"]
    .SelfDeactivate()
    .Request()
    .PostAsync();

```