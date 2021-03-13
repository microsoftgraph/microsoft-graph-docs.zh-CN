---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45254b40f7161cb509e01bbae99736b01ee148c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.Users["{user-id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```