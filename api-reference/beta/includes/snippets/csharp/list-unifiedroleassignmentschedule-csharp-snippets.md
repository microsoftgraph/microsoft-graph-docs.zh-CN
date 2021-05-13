---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6816ececa885b90685627ff7f0e6e855f6fee572
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignmentSchedules = await graphClient.RoleManagement.Directory.RoleAssignmentSchedules
    .Request()
    .GetAsync();

```