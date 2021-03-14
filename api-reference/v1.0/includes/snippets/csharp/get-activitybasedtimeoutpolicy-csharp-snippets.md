---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcf7a78bdbe1d46d1d4c3aaf66edc897d983ed02
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityBasedTimeoutPolicy = await graphClient.Policies.ActivityBasedTimeoutPolicies["{activityBasedTimeoutPolicy-id}"]
    .Request()
    .GetAsync();

```