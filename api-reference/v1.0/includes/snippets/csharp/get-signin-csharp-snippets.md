---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aa1f4d787169e5f37340ca755e6f0f75dc34d61f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var signIn = await graphClient.AuditLogs.SignIns["{id}"]
    .Request()
    .GetAsync();

```