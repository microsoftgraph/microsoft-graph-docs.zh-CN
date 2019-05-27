---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6027613007faaffb1203ce10283e1ef5b0f28b2a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461571"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addLicenses = new List<AssignedLicense>()
{
    new AssignedLicense
    {
        DisabledPlans = new List<Guid>()
        {
            "11b0131d-43c8-4bbb-b2c8-e80f9a50834a"
        },
        SkuId = "skuId-value-1"
    },
    new AssignedLicense
    {
        DisabledPlans = new List<Guid>()
        {
            "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235"
        },
        SkuId = "skuId-value-2"
    }
};

var removeLicenses = new List<Guid>()
{
};

await graphClient.Me
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```