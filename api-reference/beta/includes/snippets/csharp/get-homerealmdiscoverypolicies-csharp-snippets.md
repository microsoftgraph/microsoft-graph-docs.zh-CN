---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 701fd21ee5e5da9e2c07d617ca0287e70296c5b2bd84d80d6b907b34eee222fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278098"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicies = await graphClient.Policies.HomeRealmDiscoveryPolicies
    .Request()
    .GetAsync();

```