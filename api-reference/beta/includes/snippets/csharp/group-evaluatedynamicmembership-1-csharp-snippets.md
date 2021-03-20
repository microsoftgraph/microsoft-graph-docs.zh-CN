---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 363031f871da7accb6b500d46ac8c98c76cb4f97
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961875"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";

await graphClient.Groups["{group-id}"]
    .EvaluateDynamicMembership(memberId)
    .Request()
    .PostAsync();

```