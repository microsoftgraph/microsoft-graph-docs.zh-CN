---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 953b5d939a31544bfaa905a03e7b02aa6874d471
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.TermStore.Groups["{groupId}"]
    .Request()
    .GetAsync();

```