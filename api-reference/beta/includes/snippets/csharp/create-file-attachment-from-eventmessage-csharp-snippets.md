---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf500660433c52c8ac1973e7105cbeb0bc2822c9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544170"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "name-value",
    ContentType = "contentType-value",
    IsInline = false,
    ContentLocation = "contentLocation-value",
    ContentBytes = "contentBytes-value"
};

await graphClient.Me.Messages["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```