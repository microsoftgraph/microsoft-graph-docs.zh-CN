---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4764e589f625d9b7b2da087b0e2663ba552d93b7
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819732"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPublication = new ItemPublication
{
    Description = "One persons journey to the top of the branding management field.",
    DisplayName = "Got Brands? The story of Innocenty Popov and his journey to the top.",
    PublishedDate = new Date(1900,1,1),
    Publisher = "International Association of Branding Management Publishing",
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg",
    WebUrl = "https://www.iabm.io"
};

await graphClient.Me.Profile.Publications
    .Request()
    .AddAsync(itemPublication);

```