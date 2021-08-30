---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d42205bad2267b6f5d5e32f70f35681c4b493de0300eccb1a98654858d7ee4fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```