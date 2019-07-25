---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5724fd3f4f2876a942e153e105aca3a9b6c631f1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#Microsoft.OutlookServices.ItemAttachment"}
    },
    Name = "name-value",
    Item = "message or event entity"
};

await graphClient.Me.Events["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```