---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d273c3a0446a7ad0059db40981691fb5097ac12
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879518"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#microsoft.graph.referenceAttachment"}
    },
    Name = "Personal pictures",
    SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
    ProviderType = "oneDriveConsumer",
    Permission = "Edit",
    IsFolder = "True"
};

await graphClient.Me.Messages["AAMkAGE1M88AADUv0uFAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```