---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c77ecc3793f230c30475785c1c87b26b5d606d6a7e39e3a290dc1f778a51a118
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addLicenses = new List<AssignedLicense>()
{
    new AssignedLicense
    {
        DisabledPlans = new List<Guid>()
        {
            Guid.Parse("11b0131d-43c8-4bbb-b2c8-e80f9a50834a")
        },
        SkuId = Guid.Parse("guid")
    }
};

var removeLicenses = new List<Guid>()
{
    Guid.Parse("bea13e0c-3828-4daa-a392-28af7ff61a0f")
};

await graphClient.Me
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```