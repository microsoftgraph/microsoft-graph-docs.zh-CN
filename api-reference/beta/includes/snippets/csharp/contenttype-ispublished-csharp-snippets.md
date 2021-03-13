---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e0f4173b28754e570b91da24212fc3d812c355d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770571"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var boolean = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .IsPublished()
    .Request()
    .GetAsync();

```