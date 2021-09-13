---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53f21d8d5b20a0bf931d6d5605a71aee656a8ee4620b69e70d66ab6a680ddf73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221386"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicies = await graphClient.ServicePrincipals["{servicePrincipal-id}"].HomeRealmDiscoveryPolicies
    .Request()
    .GetAsync();

```