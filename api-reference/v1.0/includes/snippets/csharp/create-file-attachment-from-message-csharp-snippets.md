---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 32e3a3513c76a073e88869b2aa1cc4b99242c897
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#microsoft.graph.fileAttachment"}
    },
    Name = "smile",
    ContentBytes = "base64R0lGODdhEAYEAA7"
};

await graphClient.Me.Messages["AAMkpsDRVK"].Attachments
    .Request()
    .AddAsync(attachment);

```