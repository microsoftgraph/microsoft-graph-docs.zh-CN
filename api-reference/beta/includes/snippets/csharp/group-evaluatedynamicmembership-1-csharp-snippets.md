---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77a5d8eb5f095a967ce635d4be532ed8bfbc4b1eeb0bcad66beb6f7988a7a107
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279080"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";

await graphClient.Groups["{group-id}"]
    .EvaluateDynamicMembership(memberId)
    .Request()
    .PostAsync();

```