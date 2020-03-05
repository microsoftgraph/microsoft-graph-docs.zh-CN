---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 991d265068774da19de0b6590262e56413c9d6ca
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicies = await graphClient.ServicePrincipals["{id}"].HomeRealmDiscoveryPolicies
    .Request()
    .GetAsync();

```