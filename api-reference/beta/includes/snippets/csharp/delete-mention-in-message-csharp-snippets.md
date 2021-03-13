---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33e4f1e20f92e1505016c24f8d98e748873275da
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796618"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"].Mentions["{mention-id}"]
    .Request()
    .DeleteAsync();

```