---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28e1e78ca2fee80fe64acd70be153719f83d6ed6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791639"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"]
    .CreateReply(null,null)
    .Request()
    .PostAsync();

```