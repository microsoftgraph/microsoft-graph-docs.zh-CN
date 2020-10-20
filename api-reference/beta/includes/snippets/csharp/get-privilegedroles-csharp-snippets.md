---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a0de92a6ede3449e4ebcb969ec8449b709954a5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611405"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoles = await graphClient.PrivilegedRoles
    .Request()
    .GetAsync();

```