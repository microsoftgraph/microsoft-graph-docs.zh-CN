---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0b07faa09a4ad952dac15b03023b4ac4feff510
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604774"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.PrivilegedRoles["{id}"].Assignments
    .Request()
    .GetAsync();

```