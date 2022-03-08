---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2812f4ba032ee5c3fe7db8f671e3ab4b605397a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336807"
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
        SkuId = Guid.Parse("45715bb8-13f9-4bf6-927f-ef96c102d394")
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