---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2ebdf3cb42d99826aafa806f962a2d52dfeef894
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463618"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    Name = "menu.txt",
    ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
};

await graphClient.Me.Events["AAMkAGI1AAAt9AHjAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```