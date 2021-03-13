---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cfa21c6d84fe8f7ba43e2b8d34d1496b57b7191
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785941"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = await graphClient.Teams["{team-id}"].Members["{conversationMember-id}"]
    .Request()
    .GetAsync();

```