---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 699c90c6148315b2b0d46b9ebc9fd8a475d05a8b
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.ClaimsMappingPolicies["{id}"]
    .Request()
    .DeleteAsync();

```