---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65ca6e12909343d42e8deda0e3bef083cfb31d71
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43718470"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityBasedTimeoutPolicies = await graphClient.Policies.ActivityBasedTimeoutPolicies
    .Request()
    .GetAsync();

```