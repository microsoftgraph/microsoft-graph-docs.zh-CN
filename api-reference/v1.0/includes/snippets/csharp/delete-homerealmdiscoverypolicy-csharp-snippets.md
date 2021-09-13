---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e98868c7774ad62715a3784405a5138afcb179bba76ae29b7e1fa482e27f169
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.HomeRealmDiscoveryPolicies["{homeRealmDiscoveryPolicy-id}"]
    .Request()
    .DeleteAsync();

```