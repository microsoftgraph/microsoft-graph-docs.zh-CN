---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c21fc9d75e71721cf6669d667eb04167555c10c7
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805406"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.TokenIssuancePolicies["{id}"]
    .Request()
    .DeleteAsync();

```