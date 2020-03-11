---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c21fc9d75e71721cf6669d667eb04167555c10c7
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591731"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.TokenIssuancePolicies["{id}"]
    .Request()
    .DeleteAsync();

```