---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a53f5f075076adf797370dc0a4ba6b268b717b8
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806287"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityBasedTimeoutPolicy = await graphClient.Policies.ActivityBasedTimeoutPolicies["{id}"]
    .Request()
    .GetAsync();

```