---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80460989e5bce65f8c0c279953068b754de04bfc
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "smile",
    ContentBytes = "R0lGODdhEAYEAA7"
};

await graphClient.Me.Messages["AAMkpsDRVK"].Attachments
    .Request()
    .AddAsync(attachment);

```