---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0450d3e0a0736cdc86ada7bcc5527ee43b85c6ad
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personCertification = new PersonCertification
{
    CertificationId = "KB-1235466333663322",
    Description = "Blackbelt in Marketing - Brand Management",
    DisplayName = "Marketing Blackbelt - Brand Management",
    ThumbnailUrl = "https://iame.io/dfhdfdfd334.jpg",
    WebUrl = "https://www.iame.io/blackbelt"
};

await graphClient.Me.Profile.Certifications
    .Request()
    .AddAsync(personCertification);

```