---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fcf38c0732c4430abd762c418a40e6fbad7846725595e87336152e72deb2b0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215853"
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

await graphClient.Me.Events["{event-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```