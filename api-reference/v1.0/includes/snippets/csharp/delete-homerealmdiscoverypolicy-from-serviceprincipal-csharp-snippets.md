---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0ff63c7a9905778daaa9a1149cfbc87c3cd62be
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].HomeRealmDiscoveryPolicies["{id}"].Reference
    .Request()
    .DeleteAsync();

```