---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d68c48222ad799d9f6e7549dfe0eee61efae57d7
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.ActivityBasedTimeoutPolicies["{id}"]
    .Request()
    .DeleteAsync();

```