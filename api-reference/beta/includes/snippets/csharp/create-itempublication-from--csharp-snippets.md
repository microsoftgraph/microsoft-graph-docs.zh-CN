---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 925294907b8c3d351e3c86349aab306e1ac6e96bcead2ea792f436a69224d60a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164082"
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