---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0678d1524a119bd397c6fa99703ee5865ddefc47
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209649"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrants = await graphClient.Teams["{team-id}"].PermissionGrants
    .Request()
    .GetAsync();

```