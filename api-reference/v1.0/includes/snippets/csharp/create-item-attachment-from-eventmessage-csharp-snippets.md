---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fd8537d7e3a4fdad4c1187d372189e082699431
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544208"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new ItemAttachment
{
    Name = "name-value",
    Item = "message or event entity"
};

await graphClient.Me.Events["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```