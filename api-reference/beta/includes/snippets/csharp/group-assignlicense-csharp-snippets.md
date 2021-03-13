---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef29c2440a5d1338c1d7a97a8969526f1b5d5c83
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797140"
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
        SkuId = Guid.Parse("skuId-value-1")
    },
    new AssignedLicense
    {
        DisabledPlans = new List<Guid>()
        {
            Guid.Parse("a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235")
        },
        SkuId = Guid.Parse("skuId-value-2")
    }
};

var removeLicenses = new List<Guid>()
{
};

await graphClient.Groups["{group-id}"]
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```