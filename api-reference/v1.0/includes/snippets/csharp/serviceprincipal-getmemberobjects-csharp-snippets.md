---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21e726c752be5a36f3ea19a3ccb89694fee48406b47e7c3694fab32ea2b9c95d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162365"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```