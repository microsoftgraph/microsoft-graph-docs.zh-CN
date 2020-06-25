---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 991d265068774da19de0b6590262e56413c9d6ca
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicies = await graphClient.ServicePrincipals["{id}"].HomeRealmDiscoveryPolicies
    .Request()
    .GetAsync();

```