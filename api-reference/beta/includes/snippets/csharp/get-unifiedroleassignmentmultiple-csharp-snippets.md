---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb1efe63e1924cb83fdcfb101db9b1a6b219eba6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44338925"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.DeviceManagement.RoleAssignments
    .Request()
    .Filter(" principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')")
    .GetAsync();

```