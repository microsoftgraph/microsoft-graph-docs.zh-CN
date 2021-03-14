---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e75ee2b88be72090003d5d38b8617d672f51ac5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807260"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScore = await graphClient.Security.SecureScores["{secureScore-id}"]
    .Request()
    .GetAsync();

```