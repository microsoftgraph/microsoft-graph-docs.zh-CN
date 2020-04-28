---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f92b275432b719f621d3d988213da23b8b7e5108
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43718544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicies = await graphClient.Policies.TokenLifetimePolicies
    .Request()
    .GetAsync();

```