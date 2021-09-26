---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb1efe63e1924cb83fdcfb101db9b1a6b219eba6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59764872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.DeviceManagement.RoleAssignments
    .Request()
    .Filter(" principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')")
    .GetAsync();

```