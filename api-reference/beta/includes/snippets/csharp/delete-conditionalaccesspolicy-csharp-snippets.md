---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ca346effc9a93aa67747329d766222ba9fa8c65
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ConditionalAccess.Policies["{id}"]
    .Request()
    .DeleteAsync();

```