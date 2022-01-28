---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03d6827e496cc88096b1b650d268a37ec2aa482727451624574649393f91394e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].HomeRealmDiscoveryPolicies["{homeRealmDiscoveryPolicy-id}"].Reference
    .Request()
    .DeleteAsync();

```