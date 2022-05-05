---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 957d4cf9d5f6d020674e931e7407c3779b233e51
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211497"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var documentSetVersion = new DocumentSetVersion
{
    Comment = "v1",
    ShouldCaptureMinorVersion = false
};

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].DocumentSetVersions
    .Request()
    .AddAsync(documentSetVersion);

```