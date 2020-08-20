---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78d6724161b57f72d815eaaf82da64f4a0fdcf88
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819563"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAward = new PersonAward
{
    Description = "Lifetime Achievement award from the International Association of Branding Managers",
    DisplayName = "Lifetime Achievement Award For Excellence in Branding",
    IssuedDate = new Date(1900,1,1),
    IssuingAuthority = "International Association of Branding Management",
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg",
    WebUrl = "https://www.iabm.io"
};

await graphClient.Me.Profile.Awards
    .Request()
    .AddAsync(personAward);

```