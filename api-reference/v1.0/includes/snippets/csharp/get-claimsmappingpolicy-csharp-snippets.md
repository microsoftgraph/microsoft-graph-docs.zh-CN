---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ccdf1ad5cf96275b19df213cc14a09ecea7e183
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863655"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicy = await graphClient.Policies.ClaimsMappingPolicies["{id}"]
    .Request()
    .GetAsync();

```