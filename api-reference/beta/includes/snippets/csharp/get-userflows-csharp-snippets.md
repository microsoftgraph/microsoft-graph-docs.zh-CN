---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbf3e98385eecb5403ef7a24ae925bb6297659da
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlows = await graphClient.Identity.UserFlows
    .Request()
    .GetAsync();

```