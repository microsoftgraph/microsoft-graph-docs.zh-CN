---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33fc20429d0ca6674fd74d56a666a441d49fef71
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52870505"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignments["{appRoleAssignment-id}"]
    .Request()
    .DeleteAsync();

```