---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3e0a139de467b0c4cde7270bc6230b47b1571893
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879732"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Attachments = new List<Attachment>()
    {
        new Attachment
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.type","#microsoft.graph.fileAttachment"}
            },
            Name = "guidelines.txt",
            ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
        }
    }
};

var comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name.";

await graphClient.Me.Messages["AAMkADA1MTAAAH5JaKAAA="]
    .CreateReplyAll(message,comment)
    .Request()
    .PostAsync();

```