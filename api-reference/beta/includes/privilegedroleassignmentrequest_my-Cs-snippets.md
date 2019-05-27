---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8ae0c4c61f0acb16c3e0ab108dc57b02f8f6f57d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var my = await graphClient.PrivilegedRoleAssignmentRequests.My()
    .Request()
    .GetAsync();

```