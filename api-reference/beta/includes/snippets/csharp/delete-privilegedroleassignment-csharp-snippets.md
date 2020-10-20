---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f1138c81ea35469c4b3adbe170109f3688a0815
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607658"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignments["{id}"]
    .Request()
    .DeleteAsync();

```