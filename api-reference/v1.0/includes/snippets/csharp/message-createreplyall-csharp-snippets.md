---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b89c0eef48dc581b66d1a281b880b24dfc2be7c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785805"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"]
    .CreateReplyAll(null,null)
    .Request()
    .PostAsync();

```