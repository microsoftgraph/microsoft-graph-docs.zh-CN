---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c930c5cb58a811bea8f36e18bda582db40e37df
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796636"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.PrivilegedRoles["{privilegedRole-id}"].Assignments
    .Request()
    .GetAsync();

```