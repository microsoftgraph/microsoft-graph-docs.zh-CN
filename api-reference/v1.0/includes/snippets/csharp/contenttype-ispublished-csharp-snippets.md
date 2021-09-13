---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e0f4173b28754e570b91da24212fc3d812c355d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var boolean = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .IsPublished()
    .Request()
    .GetAsync();

```