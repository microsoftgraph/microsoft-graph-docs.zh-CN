---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fd39085eece59d67150ad58d22d5ea6c6a1714384e278c9bc16fdef218a4010
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "smile",
    ContentBytes = Encoding.ASCII.GetBytes("a0b1c76de9f7=")
};

await graphClient.Me.Messages["{message-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```