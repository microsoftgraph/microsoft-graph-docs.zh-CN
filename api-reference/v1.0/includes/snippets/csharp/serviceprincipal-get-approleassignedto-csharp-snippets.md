---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 018f3543b3d8d5ba8b4fd06cb18fd69a57982566987e08bdc34abef3e107fba0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903870"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignedTo = await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignedTo
    .Request()
    .GetAsync();

```