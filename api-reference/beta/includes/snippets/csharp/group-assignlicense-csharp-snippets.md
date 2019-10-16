---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2af0fe1580fd75ee2b288932176b85374de3a40a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535581"
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

await graphClient.Groups["1ad75eeb-7e5a-4367-a493-9214d90d54d0"]
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```