---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc500a3a871c48bd4e53d43b51acc4fa3bcad1ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802734"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var projectParticipation = await graphClient.Me.Profile.Projects["{projectParticipation-id}"]
    .Request()
    .GetAsync();

```