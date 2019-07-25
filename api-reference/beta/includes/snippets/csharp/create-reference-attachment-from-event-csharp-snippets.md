---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3fa4180fbdf43ab37f50e22d6679a2bbc76b4143
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859504"
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

await graphClient.Me.Events["AAMkAGE1M88AADUv0uAAAG="].Attachments
    .Request()
    .AddAsync(attachment);

```