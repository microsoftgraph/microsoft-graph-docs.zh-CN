---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d4038b9c4c7fb65162132fc88776997472a976d
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicies = await graphClient.Policies.TokenIssuancePolicies
    .Request()
    .GetAsync();

```