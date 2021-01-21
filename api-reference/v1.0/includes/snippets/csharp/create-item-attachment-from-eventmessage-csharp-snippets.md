---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b74be9e1cbd758c6bd8acea68c9dea01ad408592
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new ItemAttachment
{
    Name = "name-value",
    Item = new Message
    {
    }
};

await graphClient.Me.Events["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```