---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43c336d9fe1fa359cf0f4437ba28ac9a8cd9524cbb0e727ecc1953b34c663f36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignments["{appRoleAssignment-id}"]
    .Request()
    .DeleteAsync();

```