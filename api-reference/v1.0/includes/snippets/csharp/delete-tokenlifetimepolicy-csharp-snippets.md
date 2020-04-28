---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7efa60a02d7da9db7f2821155606f09bdafa7646
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.TokenLifetimePolicies["{id}"]
    .Request()
    .DeleteAsync();

```