---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 859e09b3f0f036b70e95ac0605e24f3afdbf12d6
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "smile",
    ContentBytes = Encoding.ASCII.GetBytes("a0b1c76de9f7=")
};

await graphClient.Me.Messages["AAMkpsDRVK"].Attachments
    .Request()
    .AddAsync(attachment);

```