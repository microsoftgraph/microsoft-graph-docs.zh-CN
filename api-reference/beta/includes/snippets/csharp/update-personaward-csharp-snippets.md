---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 669011f7d204c01d522e9c8cbc5594d5fdd1d6ab16610deefe8dae70dec5636f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAward = new PersonAward
{
    IssuingAuthority = "International Association of Branding Management",
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
};

await graphClient.Users["{user-id}"].Profile.Awards["{personAward-id}"]
    .Request()
    .UpdateAsync(personAward);

```