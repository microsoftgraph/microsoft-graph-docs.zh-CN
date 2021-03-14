---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6376425f26d907b1b978f3b71ace847951e2286a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790075"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Messages["{message-id}"].Attachments
    .Request()
    .GetAsync();

```