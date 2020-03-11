---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0ff63c7a9905778daaa9a1149cfbc87c3cd62be
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].HomeRealmDiscoveryPolicies["{id}"].Reference
    .Request()
    .DeleteAsync();

```