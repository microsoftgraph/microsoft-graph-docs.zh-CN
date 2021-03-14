---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecce277f73fbe3f797871546bb2750087f7225e8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.Groups["{group-id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```