---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43d8c59e16235e512f21c6928ae6bb43dab63594
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202049"
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