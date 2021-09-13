---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0773bceab851ea3dc12e9b9795005dc82060a3745ef88e150f7465d9f3abfcde
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278448"
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