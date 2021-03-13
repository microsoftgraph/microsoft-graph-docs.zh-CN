---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a91402f194cdb950c6230bdccf0d4f34ef9b25f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSummary = await graphClient.PrivilegedRoles["{privilegedRole-id}"].Summary
    .Request()
    .GetAsync();

```