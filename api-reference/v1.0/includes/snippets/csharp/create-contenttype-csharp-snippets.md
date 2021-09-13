---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43d8c59e16235e512f21c6928ae6bb43dab63594
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentType = new ContentType
{
    Name = "docSet",
    Description = "custom docset",
    Base = new ContentType
    {
        Name = "Document Set",
        Id = "0x0120D520"
    },
    Group = "Document Set Content Types"
};

await graphClient.Sites["{site-id}"].ContentTypes
    .Request()
    .AddAsync(contentType);

```